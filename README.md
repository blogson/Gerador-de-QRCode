# Gerador de QRCode com jQuery / JavaScript
Script para gerar QRCode a partir do serviço público do Google Charts.
Sem dúvidas esta é uma das maneiras mais fáceis de se gerar um QRCode.

## Exemplo completo, teste o código on-line.
Você pode ver uma descrição detalhada de como utilizar este código em seus formulários HTML lendo este artigo do Blogson - 
 [Como criar um gerador de QR Code com jQuery / JS, Muito Fácil](https://www.blogson.com.br/como-criar-um-gerador-de-qr-code-com-jquery-js-facil/)

## Exemplo de formulário
O formulário precisa apenas de um textarea, um botão e um elemento de imagem.

```
<textarea maxlength="256" rows="3" id="conteudoQRCode"></textarea>
<br/>
<button type="button">
   Gerar QR Code
</button>
<img id="imageQRCode" src="...">
```

## Gerador de QRCode com jQuery
Se você prefere manipular elementos da sua página com jQuery, pode usar este código;

```
$('button').click(function() 
{
  var conteudo = $('#conteudoQRCode').val();
  var GoogleCharts = 'https://chart.googleapis.com/chart?chs=500x500&cht=qr&chl=';
  var imagemQRCode = GoogleCharts + conteudo;
  $('#imageQRCode').attr('src', imagemQRCode);
});
```

## Gerador de QRCode com JavaScript
Se você prefere manipular elementos da sua página com jQuery, pode usar este código;
