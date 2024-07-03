https://www.youtube.com/watch?v=xDHhZqWtOq8&ab_channel=OnlineTutorials

CSS:
.container:

Define um container com largura fixa de 600px, altura de 500px e preenchimento interno (padding) de 50px.
A cor do texto dentro deste container é definida como cinza (#555).
.container .content:

Define um estilo para os elementos com a classe content dentro do container.
Esses elementos têm a propriedade display definida como none, tornando-os inicialmente ocultos.
Eles também têm uma margem superior de 20px.
.container .content.contentEnglish:

Define um estilo específico para os elementos com as classes content e contentEnglish.
Esses elementos têm a propriedade display definida como block, fazendo com que sejam exibidos quando o idioma inglês é selecionado.
.check:

Define um estilo para os elementos com a classe check.
Define a posição como relativa e uma largura de 50px.
.check::before:

Cria um pseudo-elemento antes do elemento .check.
Este pseudo-elemento é um círculo com largura de 50px, altura de 25px e cor de fundo cinza (#333), simulando um botão desativado.
.check:checked::before:

Altera a cor de fundo do pseudo-elemento para azul (#00a1ff) quando o checkbox está marcado.
.check::after:

Cria um pseudo-elemento após o elemento .check.
Este pseudo-elemento é uma bola branca que simula o botão deslizante do checkbox.
Inicialmente, está posicionado à esquerda (left: 0px) do pseudo-elemento ::before.
.check:checked::after:

Move o pseudo-elemento para a direita (left: 25px) quando o checkbox está marcado, simulando a ação de deslizar.
.check:checked ~.content.contentEnglish:

Define as regras de estilo para os elementos com a classe contentEnglish que estão precedidos por um .check marcado.
Especificamente, oculta o conteúdo em inglês quando o checkbox é marcado.
.check:checked ~.content.contentPortugues:

Define as regras de estilo para os elementos com a classe contentPortugues que estão precedidos por um .check marcado.
Especificamente, exibe o conteúdo em português quando o checkbox é marcado.
.en e .pt:
Definem as cores do texto para os elementos com as classes en (inglês) e pt (português), respectivamente.
HTML:
.container:

Um contêiner que envolve todo o conteúdo.
Contém um checkbox para alternar entre os idiomas inglês e português.
<span class="en">English</span> e <span class="pt">pt-BR</span>:

Links de idioma para inglês e português.
.content.contentEnglish e .content.contentPortugues:

Blocos de conteúdo que contêm texto em inglês e português, respectivamente.
Apenas um deles é exibido de cada vez, dependendo do estado do checkbox.