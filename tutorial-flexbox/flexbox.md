# Flexbox

O Flexbox é um conjunto de ferramentas para a criação de layouts e grids responsivos de forma mais fácil e rápida. Para começarmos a usar precisamos incluir dentro da classe do elemento a propriedade `display: flex`.

Materiais de apoio sobre Flexbox para aprofundarem os seus conhecimentos. Sugestões:

- https://origamid.com/projetos/flexbox-guia-completo/
- https://developer.mozilla.org/pt-BR/docs/Learn/CSS/CSS\_layout/Flexbox (em inglês)
- https://philipwalton.github.io/solved-by-flexbox/ (em inglês)

### **Uma volta rápida ao passado**

Antigamente utilizávamos o float para desenvolver grids de páginas, posicionar uma imagem e texto um ao lado do outro, mas você sabe qual é a real utilidade dele? O certo é usarmos quando precisamos determinar que um elemento deve ser retirado do seu fluxo normal e colocado ou no lado direito ou esquerdo fazendo com que ele "flutue" dentro do content.

Assim como float outra propriedade que era utilizada bastante era o position para trabalharmos com posicionamentos verticais, por exemplo.

Com o Flexbox não precisamos mais usá-los para estruturar grids.

### **Propriedades do Flexbox**

O Flexbox oferece várias propriedades que ajudam no processo de desenvolvimento de grids. Para começar a utilizar você precisa adicionar a propriedade `display: flex` dentro da classe do seu elemento. Com o flex nós fazemos com que todos os elementos filhos da da classe pai em flex itens, podendo então trabalhar com as outras propriedades flex.

Outras propriedades do Flexbox:
- https://origamid.com/projetos/flexbox-guia-completo/

As propriedades vamos usar no nosso desafio são essas:

- **flex-direction:** define que tipo de direção o nosso flex item vai seguir, se ele vai ter um tipo linha \(row, row-reverse\) ou coluna \(column, column-reverse\);
- **flex-wrap**: define se os itens devem quebrar ou não a linha. Usando o wrap você determina que essa quebra seja realizada;
- **justify-content**: define o posicionamento dos elementos, seja à esquerda \(flex-start\), ao centro \(center\), à direita \(flex-end\) ou alinhando entre os dois lados \(esquerda e direita\) de forma fluída \(space-between\).

A propriedade `justify-content` acaba substituindo e agindo de maneira correta o posicionamento dos elementos seja um lado do outro, ao centro, à esquerda ou direita, de forma flexível.
