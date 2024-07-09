<h1>Reconhecimento de Gestos com as Mãos usando OpenCV</h1>
Este projeto em Python utiliza o OpenCV para reconhecer gestos da mão em tempo real a partir da captura de vídeo da webcam. Ele detecta gestos como números e associa cada gesto a uma ação específica, como abrir um programa no computador.

<h2>Pré-requisitos</h2>
<ul>
  <li>Python 3.x</li>
<li>OpenCV (cv2)</li>
<li>NumPy</li>
<li>Biblioteca Math</li>
</ul>

<h2>Funcionalidades</h2>
  <h3>Detecção de Gestos da Mão:</h3>
  <li>Converte o espaço de cores BGR para HSV para melhor detecção de pele.</li>
  <li>Cria uma máscara para isolar a região da mão com base no tom de pele.</li>
  <li>Identifica contornos e constrói um casco convexo ao redor da mão.</li>
  <li>Reconhece gestos com base nos defeitos no casco convexo e exibe a ação correspondente na tela.</li>
  
  <h3>Interface de Usuário:</h3>
  <li>Mostra o feed de vídeo da webcam com feedback visual dos gestos reconhecidos.</li>
  <li>Textos indicativos dos gestos e suas ações são exibidos diretamente no vídeo.</li>
