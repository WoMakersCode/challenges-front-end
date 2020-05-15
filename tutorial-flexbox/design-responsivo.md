# Design Responsivo

Em tempos atuais desenvolver telas responsivas já faz parte do cotidiano de uma pessoa desenvolvedora front-end. Mas para quem está começando o que é o design responsivo?  
  
O termo "Responsive Web Design" \(Web Design Responsivo\) é um conceito criado em meados de 2010 por [Ethan Marcotte](https://alistapart.com/article/responsive-web-design). A técnica nada mais é do que o usar o layout de uma página na web e ajustá-lo automaticamente com base no tamanho das telas dos usuários.  
  
Então podemos dizer que cada bloco de elemento de uma página \(imagem, textos, animações\) possuem comportamentos diferentes quando estão em telas maiores \(desktop\) e em telas menores \(tablets, celulares\).  
  
E como você faz para tornar o seu site responsivo? Através da tag Viewport.  
  
A tag Viewport é responsável por nos permitir que o nosso site torne-se responsivo e que nos permita usar media queries \(veremos sobre isso mais a frente\). Usamos ela dentro da nossa tag &lt;head&gt;, pois no momento em que a página está sendo carregada ele será "chamado" permitindo com que meus blocos de elementos possam se comportar de maneira diferente de acordo com o tamanho da tela.  
  
Para implementá-lo basta você incluído dentro da tag &lt;head&gt;. Assim:

```markup
<html>
   <head>
      <title>Meu site pessoal</title>
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
   </head>
</html>
```

O width=device-width usamos ele para declarar que a nossa tela irá de se adaptar de acordo com a tela do dispositivo. Sem ele a nossa página ficaria do tamanho conforme a pessoa desenvolvedora iria adaptar.    
  
O initial-scale=1.0 usamos ele para declarar o nível de zoom inicial da página quando carregada pelo navegador.  
  
Lá na frente você verá melhor na prática quando implementar o desafio.

