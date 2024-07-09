Reconhecimento de Gestos com as Mãos usando OpenCV
Este projeto demonstra o reconhecimento de gestos em tempo real usando OpenCV em Python. Ele detecta vários gestos da mão com base nos contornos e casco convexo da região da mão.

Requisitos
  Python 3.x
  OpenCV (cv2)
  NumPy
  Biblioteca Math
  Instalação
  Certifique-se de ter o Python instalado no seu sistema. Instale o OpenCV e NumPy usando pip se ainda não estiverem instalados:

bash
  pip install opencv-python numpy

bash
  git clone <URL-do-repositório>
  cd <diretório-do-repositório>
Executar o Script:

bash
  python reconhecimento_gestos.py
  Funcionamento
  O script captura frames da sua webcam (cv2.VideoCapture(0)) e realiza as seguintes etapas:

Pré-processamento do Frame:

Inverte horizontalmente o frame para facilitar a interação do usuário.
Define uma região de interesse (ROI) para detectar gestos da mão.
Detecção de Gestos da Mão:

Converte a ROI do espaço de cores BGR para HSV para melhor detecção do tom de pele.
Cria uma máscara binária para isolar a região da mão usando um intervalo de cores HSV pré-definido.
Aprimora a máscara usando dilatação e desfoque gaussiano.
Cálculo de Contorno e Casco Convexo:

Encontra os contornos da mão na imagem mascarada.
Aproxima o contorno para um polígono mais simples.
Constrói um casco convexo ao redor do contorno da mão.
Reconhecimento de Gestos:

Identifica defeitos no casco convexo para reconhecer gestos da mão.
Classifica os gestos com base no número de defeitos detectados.
Exibe texto correspondente no frame para gestos reconhecidos.
Interação do Usuário:

Mostra o frame processado com texto indicando o gesto reconhecido.
Pressione a tecla Esc para sair do programa.
Observações
Certifique-se de que sua webcam esteja corretamente configurada e funcional.
