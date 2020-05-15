# Mobile First

Dentro do nosso tópico sobre design responsivo existe um outro conceito chamado Mobile First que determina que para um desenvolvimento mais escalável deveríamos primeiro escrever o nosso código para versões menores \(mobile, tablets\) e depois para maiores \(desktop\), ou seja, em ordem crescente.  
  
Para facilitar melhor o entendimento como seria esse conceito na prática segue o exemplo de um código CSS:

```css
p {
     font-size: 1rem;
}

@media (min-width: 768px) {
     p {
         font-size: 1.5rem;
      }
}
```

No exemplo acima determinamos que a nossa tag &lt;p&gt; até a resolução 767px possuirá 1rem \(16px\) e a partir do 768px terá o tamanho 1.5rem \(24px\).    
  
Caso tenha ficado confuso para você acima, o rem é uma medida que usamos no CSS para trabalhar com responsividade, pois nos ajuda a deixar o código mais flexível facilitando o site conseguir se adequar a determinadas resoluções.  
  
O cálculo do rem consiste em atribuir um valor definido na raiz \(por isso o R = root em\) e a partir daí definirmos o tamanho das outras fontes pegando o valor dela em px e dividir pelo valor que atribuímos por lá \(por padrão usamos 16px\) para convertermos em rem. A raiz costuma ser a tag html.  
Por exemplo: precisamos determinar o tamanho do nosso &lt;p&gt; em telas maiores. Em px ele tem 24. Pegamos o 24 e dividirmos por 16 que resultará em 1.5.  

### **Qual é a diferença entre o design responsivo e adaptativo?**

É muito comum ver pessoas confundindo sites adaptativos com responsivos. Mas o conceito de ambos são diferentes.  
  
O design adaptativo usa layouts específicos para cada breakpoint \(ponto de quebra\), ou seja, no desktop possui um layout e no mobile é um outro completamente diferente. Passando isso para o código teríamos que detectar qual é a resolução que o usuário está usando e carregar um layout apropriado para ele.    
  
Já o responsivo é completamente diferente disso. Não precisamos ficar criando layouts exclusivos para um determinado tipo de dispositivo. A ideia é que o layout vá se adaptando de acordo com a tela a ser usada e isso dentro do código, não ter 3 páginas HTML diferentes para desktop outro para tablet e um para o mobile. Apenas 1 código HTML que suporte essas resoluções manipulando os seus comportamentos através do CSS e dependendo da situação com o uso do Javascript também.  
****

