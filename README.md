UnB - Universidade de Brasilia  
FGA - Faculdade do Gama  
TPPE - Técnicas de Programação para Plataformas Emergentes  

### Trabalho Prático 2 - _Qualidade do projeto de código_

---

**Participantes**

- Victor Souza Dantas Martins Lima - 190044403
- Vitor Magalhães Lamego - 190020903


## Simplicidade

### Descrição: 

A simplicidade no projeto de software diz respeito à busca pela clareza, concisão e facilidade de compreensão do código. Um código simples é aquele que apresenta uma estrutura lógica e organizada, facilitando sua leitura, manutenção e teste.

**Efeitos no código:** A simplicidade impacta a estrutura do código, tornando-o mais legível e compreensível. Métodos curtos e bem nomeados, classes coesas e bem encapsuladas, além de uma estrutura de controle de fluxo direta e sem ramificações complexas, são alguns dos efeitos da simplicidade no código.

### Relação com maus cheiros de código:

**Código duplicado:** A busca pela simplicidade incentiva a eliminação de código duplicado. 

**Método longo:** A simplicidade favorece a quebra de métodos longos em métodos menores e mais coesos. 

**Intimidade inapropriada:** A simplicidade promove a redução do acoplamento desnecessário entre classes.

### Operação de refatoração:

A operação de refatoração Extract Method é uma técnica útil para alcançar a simplicidade. Ao identificar trechos de código complexos dentro de um método, você pode extrair esse trecho em um novo método, dando-lhe um nome descritivo. Isso reduz a complexidade do método original e melhora a clareza do código.

## Elegância

### Descrição: 

A elegância no projeto de software está relacionada à qualidade estética do código. Um código elegante é aquele que segue as melhores práticas de programação, é bem estruturado, expressivo e eficiente.

**Efeitos no código:** A busca pela elegância resulta em um código mais estruturado e fácil de ler. O uso adequado de padrões de design, nomes significativos para variáveis e métodos, bem como a eliminação de soluções complexas ou redundantes, são exemplos dos efeitos da elegância no código.

### Relação com maus cheiros de código:

**Código duplicado:** A eliminação de código duplicado é uma prática que contribui para a elegância do código. 

**Método longo:** A elegância busca a redução de métodos longos e complexos. 

**Comentários:** Um código elegante e autoexplicativo elimina a necessidade de comentários excessivos e desnecessários.

### Operação de refatoração:

A operação de refatoração Extract Method é uma ferramenta importante para eliminar a duplicação de código. Ao identificar trechos de código repetidos, você pode extrair essas partes para um método separado e, em seguida, chamar esse método em vez de repetir o código duplicado. Essa refatoração ajuda a melhorar a elegância e a manutenibilidade do código.

## Modularidade (baixo acoplamento e alta coesão)

### Descrição: 

A modularidade diz respeito à organização do código em módulos independentes e reutilizáveis. Um código modular é caracterizado por baixo acoplamento, ou seja, poucas dependências entre módulos, e alta coesão, onde cada módulo possui uma responsabilidade clara e bem definida.

**Efeitos no código:** A modularidade resulta em um código mais flexível e fácil de manter. A separação das funcionalidades em módulos distintos reduz a complexidade global do sistema e permite que as alterações sejam feitas de forma isolada, minimizando os efeitos colaterais.

### Relação com maus cheiros de código:

**Classe inchada:** A modularidade busca evitar a classe inchada, que possui muitas responsabilidades.

**Lista de parâmetros longa demais:** A modularidade favorece a redução da lista de parâmetros de um método, pois muitos parâmetros podem indicar uma responsabilidade excessiva. 

**Classes alternativas com diferentes interfaces:** A modularidade incentiva a padronização de interfaces entre classes alternativas. 

### Operação de refatoração:

A operação de refatoração Extract Class pode ser usada para mover responsabilidades relacionadas a uma nova classe. Ao identificar que uma classe está com baixa coesão, você pode extrair as responsabilidades não relacionadas para uma nova classe. Isso ajuda a reduzir o acoplamento e aumentar a coesão entre as classes.

## Boas interfaces

### Descrição:

Boas interfaces no projeto de software referem-se à definição de interfaces claras e bem projetadas que estabelecem contratos entre os componentes. Uma boa interface deve ser simples, intuitiva e fornecer apenas os métodos e propriedades necessários para interagir com um componente.

**Efeitos no código:** A definição de boas interfaces melhora a comunicação e a interação entre os componentes do sistema. Interfaces bem projetadas facilitam o uso correto dos componentes e permitem a substituição de implementações sem afetar o código que os utiliza.

### Relação com maus cheiros de código:

**Mudanças divergentes:** Boas interfaces fornecem contratos estáveis e bem definidos, evitando mudanças divergentes em várias partes do código. 

**Homem do meio:** Interfaces claras e bem definidas ajudam a evitar o mau cheiro do homem do meio, onde uma classe se torna um intermediário desnecessário entre outras classes. A definição adequada das interfaces permite uma comunicação direta e eficiente entre as classes envolvidas.

**Biblioteca de classes incompletas:** Interfaces bem projetadas garantem que as classes implementem todos os métodos necessários, evitando bibliotecas de classes incompletas.

### Operação de refatoração:

A operação de refatoração Extract Interface pode ser usada para definir interfaces mais específicas e granulares. Ao identificar que uma interface possui métodos que não são necessários em todos os contextos de uso, você pode extrair uma nova interface com os métodos relevantes. Isso ajuda a remover métodos desnecessários de uma interface e reduzir a dependência de funcionalidades não utilizadas.

## Ausência de duplicidades

### Descrição: 

A ausência de duplicidades refere-se à prática de evitar a repetição desnecessária de código. O código duplicado dificulta a manutenção, aumenta a probabilidade de erros e viola o princípio "Don't Repeat Yourself" (DRY).

**Efeitos no código:** A ausência de duplicidades resulta em um código mais conciso, legível e fácil de manter. A eliminação de duplicações promove a reutilização de código, reduz a complexidade e aumenta a consistência do sistema.

### Relação com maus cheiros de código:

**Código duplicado:** A ausência de duplicidades é diretamente relacionada à eliminação de código duplicado no projeto. O mau cheiro "Código duplicado" é abordado pela busca de soluções para evitar repetições desnecessárias de trechos de código.

### Operação de refatoração:

A operação de refatoração Extract Method é uma técnica amplamente utilizada para eliminar duplicidades de código. Ao identificar trechos de código duplicados, você pode extrair essas partes para um método separado e, em seguida, chamar esse método em vez de repetir o código duplicado. Essa refatoração promove a reutilização de código, melhora a manutenibilidade e evita erros causados por alterações inconsistentes.
