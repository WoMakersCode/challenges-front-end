# Media Queries

Antes de começar a falar sobre as media queries vamos recapitular e voltar no tempo das medias types.  
  
As medias types eram usadas para definir um CSS diferente para cada tipo de dispositivo ou seja, existia um desktop.css, tablet.css e mobile.css, por exemplo. Então se você estivesse acessando um site no tablet o media type detectava qual dispositivo estava usando e redirecionava uma folha de estilo específico para aquele tipo de tela. Com a vinda das media queries tudo isso mudou.  
  
A media query é uma propriedade que determina uma condicional para cada tipo de dispositivo. Então dependendo de qual resolução você poderá incluir regras específicas para ele. Por exemplo: o elemento header possui um background-color cinza no desktop, mas no mobile a sua cor será branca. Assim:  


```css
header {
  background-color: white;
}

@media (min-width: 768px) {
  header {
    background-color: gray;
}
```

Perceba que usamos a propriedade @media determinando que a partir da largura 768px uma outra cor de fundo será exibida no header.   
  
Para declarar as media queries costumamos usar apenas o @media\(\) onde dentro dos parênteses determinamos o valor mínimo ou máximo da resolução como condicional \(min-width e max-width, respectivamente\), mas podemos usar outras propriedades ou determinar o máximo e mínimo delas juntos. Assim:

```css
@media screen and (min-width: 768px and max-width: 1024px)
```

No exemplo acima estamos determinando que para um dispositivo com um screen \(tela\) com largura entre 768px e 1024px terá customizações diferentes.  
  
Poderíamos usar sem o screen? Sim, pois os dois teoricamente possuem a mesma regra onde a única diferença é que estamos deixando mais explícito uma especificação de que as telas que possuem determinada largura irão ter um comportamento específico.

Não vamos aprofundar muito nas propriedades e regras do @media, pois nesta documentação vamos focar apenas nas mais usadas \(e que serão importantes no nosso desafio\), mas para se ter uma ideia podemos determinar largura para dispositivos mobile usando o device, especificar a orientação dele se está no modo retrato \(portrait\) ou paisagem \(landscape\), entre outros.

{% hint style="info" %}
Mentoras: recomendamos sugerir um material de apoio para as mentorandas que queiram aprofundar mais sobre as outras regras do @media. Link do W3Schools \(em inglês\):  [https://www.w3schools.com/cssref/css3\_pr\_mediaquery.asp](https://www.w3schools.com/cssref/css3_pr_mediaquery.asp)
{% endhint %}

  


