# Guia de CSS Grid

### Definição
CSS Grid é um sistema de organização de layout 2d disponível no CSS. Está na sua segunda versão (disponibilizada no CSS3). Esse gerenciador permite organizar elementos em um formato de grade.

## Aplicação
### Propriedades (tem outras mas dá pra fazer tudo com essas)

 - `grid-template-columns`: determina quantas e qual a largura das colunas da grade
 - `grid-template-rows`: determina quantas e qual a largura das linhas da grade
 - `grid-template-areas`: permite criar uma estrutura estática de grid organizada da forma como o desenvolvedor queira
 - `grid-auto-flow`: define a direção de organização dos módulos de grid, podendo ser em linhas ou colunas
 - `grid-row`: define onde inicia e termina o grid - `<inicio> / <fim>` - e/ou a mesclagem de linhas - `span <n> `
 - `grid-column`: define onde inicia e termina o grid - `<inicio> / <fim>` - e/ou a mesclagem de colunas - `span <n> `
 - `grid-area`: define o nome do módulo de grid
 - `grid-row-gap`: valor da largura da área de respiro entre colunas
 - `grid-column-gap`: valor da altura da área de respiro entre linhas
 - `grid-gap`: valor da largura/altura da área de respiro
 > algumas propriedades do `flex css` também de aplicam ao `css grid`, como é o caso de `justify-content`, `align-items`, `order`, etc.

### Funções
- `repeat()`: recebe, como primeiro parâmetro, o número de repetições (também possível utilizar`auto-fill` ou `auto-fit` para que o número de repetições seja definido automaticamente, a partir da disponibilidade de espaço); e, como segundo parâmetro, a largura/altura da coluna/linha
- `minmax()`: recebe, como primeiro parâmetro, o valor mínimo de largura/altura assumido pela coluna/linha e, em seguida, o valor máximo assumido

### Units
- `fr`: unidade de medida utilizada no grid que indica fração do espaço disponível

## Exemplos
No referido projeto, há 3 exemplos de uso de `css grid` para construir diferentes estruturas:
1. **CardList**: Exibe uma estrutura responsiva de lista de cards, onde as colunas tem uma largura fixa e se organizam, em número, de acordo com o tamanho da tela
2. **Relógio**: Demonstra uma estrutura fixa de grade, na qual os elementos se organizam de modo definir um título e distâncias iguais entre números (referentes a horas, minutos e segundos) e separadores (:)
3. **Estrutura multicoluna**: Mostra uma estrutura de página na qual se utiliza grid para definir uma estrutura de múltiplas colunas - tanto com relação ao menu lateral e ao container de conteúdo, quanto em relação á exibição dentro do container, na qual o texto é dividido em duas colunas e o título as mescla

## References
- https://css-tricks.com/snippets/css/complete-guide-grid/
- https://www.w3schools.com/css/css_grid.asp
- https://www.origamid.com/projetos/css-grid-layout-guia-completo/
- https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Grid_Layout
