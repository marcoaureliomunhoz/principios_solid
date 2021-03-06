# Princípios SOLID

Consistem em 5 princípios que podem ser aplicados em projetos de softwares orientados a objetos para que:  
- Sejam mais legíveis.
- A manutenção seja mais fácil. 
- Sejam mais estensíveis e com menor esforço possível.
- Sejam mais adequados à realização de testes automatizados.
- Possibilitem o máximo de reaproveitamento.
- Permaneçam o máximo de tempo possível no ar (em funcionamento).

Os princípios:

**Single Responsibility Principle - SRP**  
_Princípio da Responsabilidade Única_  
- Uma classe deve ter uma, e apenas uma, razão para ser modificada.

**Open/Closed Principle - OCP**  
_Princípio do Aberto/Fechado_  
- Entidades de software (classes, módulos, funções, arquivos, etc) devem estar abertas para estensão, mas fechadas para modificações. 
- Torne os atributos de uma classe privados, ou seja, não deixe que o cliente altere/modifique o estado sem acionar métodos da própria classe. 
- Tome cuidado ao permitir a sobrescrita de métodos. No C# evite usar **virtual**.

**Liskov Substitution Principle - LSP**  
_Princípio da Substituição de Liskov_  
- Objetos de uma classe devem ser substituíveis por objetos de subclasses sem problemas (herança e polimorfismo).
- Esse princípio prega a aplicação do Polimorfismo, mas nem sempre é possível aplicar o polimorfismo, por mais que pareça possível.  
- Tome cuidado com a herança. Esta só deve ser usada quando de fato existe hierarquia.
- Evite herança quando se busca apenas reaproveitamento de código (diminuição de código). Nestes casos a melhor opção é o uso de **composição/agregação**.

**Interface Segregation Principle - ISP**  
_Princípio da Segregação de Interfaces_  
- Clientes não devem ser forçados a depender de métodos que não usam ou não fazem sentido no contexto do cliente. 
- Esse princípio prega, em geral, a aplicação de interfaces mais específicas, pois geralmente a estratégia de muitas interfaces específicas é melhor do que a estratégia de uma única interface genérica. Porém tem casos em que a aplicação de interfaces genéricas também é uma boa estratégia. 

**Dependency Inversion Principle - DIP**  
_Princípio da Inversão de Dependência ou Inversão de Controle ou Injeção de Dependência_  
- Dependa de uma abstração e não de uma implementação. 
- Esse princípio prega uma maior utilização de classe abstratas e interfaces no lugar de classes concretas, pois essa estratégia ajuda a desacoplar. 
- O ideal é evitar que módulos de alto nível dependam de módulos de baixo nível. Ambos devem depender de abstrações, abstrações não devem depender de detalhes e detalhes devem depender de abstrações.  

--- 

**Fontes**  
- https://en.wikipedia.org/wiki/SOLID_(object-oriented_design) 
- https://www.youtube.com/watch?v=Q2QdkiX6p_Y (Eduardo Pires)
- https://www.youtube.com/watch?v=i9Il79a2uBU (Eduardo Pires)
- https://brizeno.wordpress.com/solid
