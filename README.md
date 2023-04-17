<h1 align="center">
  <p align="center">Projeto <a href="https://fde-galeria-imagens-j-query.vercel.app/">Galeria de Fotos</p></a>
 <img src="https://media.giphy.com/media/dwL34LIvm9TxzAVOyL/giphy.gif" alt="Pessoa tirando foto com camera antiga">
</h1>
<div style="display: inline_block"><br>
  <div align="center">
  <img align="center" alt="fde95-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="fde95-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  <img align="center" alt="fde95-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
</div>

<h3> Sobre o Projeto </h3>
No nono módulo do curso de Engenheiro Front-End oferecido pela EBAC, tivemos a intrudução ao jQuery, uma biblioteca de funções do JavaScript que interagem com páginas HTML, projetada para simplificar scripts a serem executados/interpretados no navegador de Internet do usuário.
Como exercício durante este módulo, tivemos como desafio a criação de uma galeria de fotos onde o usuário possa adicionar uma imagem a partir do URL da mesma.
Utilizando o Adobe Color, selecionei uma paleta de cores mais elegante e simplista e importei a fonte Jost do Google.
Ao clicar no botão de <b>"Nova Imagem +"</b>, é exibido um novo campo com efeito slide down para que o usuário possa adicionar uma nova imagem.
Após colar a URL da imagem no campo destinado, o usuário deve clicar no botão <b>"Adicionar"</b> e a imagem será inseria abaixo da lista de imagens existente.
Caso o usuário desista da ação, basta clicar no botão <b>"Cancelar"</b> que o campo será removido da tela com o efeito Slide Up.


<h2>Acesse aqui: <a href="https://fde-galeria-imagens-j-query.vercel.app/"><b> Galeria de Fotos. </b></a></h2>

<br></br>
<h3>Pré Visualização</h3>
<img width="600" src="https://user-images.githubusercontent.com/123211425/232518512-e9ccdac6-1dfa-4d6b-8504-cb54392de992.png">


<h4>Inclusão de uma nova imagem</h4>
<img width="600" src="https://user-images.githubusercontent.com/123211425/232518917-d9853b55-ccf3-4157-86b2-ecedc7e4a703.png">

<h4>Imagem adicionada</h4>
<img width="600" src="https://user-images.githubusercontent.com/123211425/232520203-69e802ff-17e1-4bd6-874c-d98b429835d1.png">

<br></br>

<h3>Contatos</h3>
<div style="display: inline_block">
 <a href="https://instagram.com/fde.95" target="_blank"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
 <a href = "mailto:fdespinoza95@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
 <a href="https://www.linkedin.com/in/fde95" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
</div>

<br></br>

<h3>Código Completo</h3>

<h4>HTML</h4>

```xml
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./main.css"> <!--Importação CSS-->
    <link rel="preconnect" href="https://fonts.googleapis.com"> <!--Importação Google Fonts-->
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin> <!--Importação Google Fonts-->
    <link href="https://fonts.googleapis.com/css2?family=Jost:wght@200;400;800&display=swap" rel="stylesheet"> <!--Importação Google Fonts-->
    <title>jQuery</title>
</head>
<body>
    <header>
        <h1>Galeria de Fotos</h1>
        <button type="button">Nova Imagem +</button>
    </header>
    <form>
        <h2>Inserir nova imagem</h2>
        <input type="url" id="addressNewImage" required placeholder="URL da Imagem" autocomplete="off" />
        <button type="submit">Adicionar</button>
        <button id="buttonCancel" type="reset">Cancelar</button>
    </form>
    <ul>
        <li><img src="./images/foto1.jpg" alt="pintura de um gato em óleo sobre tela"/>
            <div class="overlayImageLink">
                <a href="./images/foto1.jpg" title="Ver imagem em tamanho real" target="_blank">
                    Ver imagem em tamanho real
                </a>
            </div>
        </li>
        <li><img src="./images/foto2.jpg" alt="pintura de um gato em óleo sobre tela"/>
            <div class="overlayImageLink">
                <a href="./images/foto2.jpg" title="Ver imagem em tamanho real" target="_blank">
                    Ver imagem em tamanho real
                </a>
            </div>
        </li>
        <li><img src="./images/foto3.jpg" alt="pintura de um gato em óleo sobre tela"/>
            <div class="overlayImageLink">
                <a href="./images/foto3.jpg" title="Ver imagem em tamanho real" target="_blank">
                    Ver imagem em tamanho real
                </a>
            </div>
        </li>
        <li><img src="./images/foto4.jpg" alt="pintura de um gato em óleo sobre tela"/>
            <div class="overlayImageLink">
                <a href="./images/foto4.jpg" title="Ver imagem em tamanho real" target="_blank">
                    Ver imagem em tamanho real
                </a>
            </div>
        </li>
    </ul>
    <footer>
        &copy; Criado e Desenvolvido por - <b><a href="https://linktr.ee/fde95" title="Conecte-se comigo em outras redes" target="_blank">Felipe Espinoza</a></b> - 2023
    </footer>
    <script src="https://code.jquery.com/jquery-3.6.4.min.js"></script> <!--Importação jQuery-->
    <script src="./main.js"></script> <!--Importação JavaScript-->
</body>
</html>
```
<h4>CSS</h4>

```css
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Jost', sans-serif;
}

header{
    display: flex;
    justify-content: center;
    background-color: #1F1F26;
    padding: 16px 0;
    color: #8C8070;
    border-bottom: 16px solid #16161c;
    text-transform: uppercase;
}

header button{
    margin-left: 16px;
    border-radius: 50px;
    border: none;
    background-color: #59300C;
    color: #D9863D;
}

header button:hover{
    color: #59300C;
}


form{
    background-color: #F2E2CE;
    color: #59300C;
    padding: 20px 0;
    text-align: center;
    display: none;
}

form h2{
    margin-bottom: 16px;
    text-transform: uppercase;
}

input{
    padding: 8px;
    width: 300px;
    border-radius: 4px;
    border: none;
}

button {
    background-color: #59300C;
    color: #F2E2CE;
    border-radius: 50px;
    border: none;
    cursor: pointer;
    text-transform: uppercase;
    padding: 8px;
    font-weight: bold;
}

#buttonCancel{
    background-color: #1F1F26;
    color: #F2E2CE;
}

button:hover,
#buttonCancel:hover{
    color: #1F1F26;
    background-color: #D9863D;
}

ul{
    display: flex;
    flex-wrap: wrap;
}

ul li{
    max-width: 25%;
    list-style: none;
    position: relative;
    max-height: 250px;
    overflow-y: hidden;
}

ul li img{
    width: 100%;
}

.overlayImageLink{
    padding: 16px;
    background-color: rgba(0,0,0,0.5);
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    opacity: 0;
    transition: all ease .5s; /*Tempo de transição de animação*/
}

.overlayImageLink a{
    color: #fff;
    text-decoration: none;
}

ul li:hover .overlayImageLink{
    opacity: 1;
}

footer{
    margin-top: 360px;
    padding: 10px;
    text-align: center;
    background-color: #1F1F26;
    color: #8C8070;
}

footer a{
    text-decoration: none;
    color: #8C8070;
}

footer a:hover{
    color: #fff;
}
```

<h4>JavaScript</h4>

```js
$(document).ready(function(){
    $('header button').click(function(){
        $('form').slideDown();
    });

$('#buttonCancel').click(function(){
    $('form').slideUp();
})

    $('form').on ('submit', function(e) {
        e.preventDefault();

        const addressNewImg = $('#addressNewImage').val();
        const newItem = $('<li style="display:none"></li>');
        $(`
            <img src="${addressNewImg}" />`
        ).appendTo(newItem);

        $(`
            <div class="overlayImageLink">
                <a href="${addressNewImg}" title="Ver imagem em tamanho real" target="_blank">
                Ver imagem em tamanho real
                </a>
            </div>
        `).appendTo(newItem);

        $(newItem).appendTo('ul');
        $(newItem).fadeIn();
        $('#addressNewImage').val('');
    })
})
```
