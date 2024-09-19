# Pilares da Programação Orientada a Objetos

# Auto Anki cards

- Quais os três paradigmas de programação?
  - Programação orientada a objetos;
  - Programação procedural;
  - Programação funcional.
- O que é programação orientada a objetos (OOP)?

  Programação Orientada a Objetos (POO) é um paradigma de programação que organiza (orienta) o software em "objetos," que podem ser vistos como entidades que combinam dados (atributos ou propriedades) e comportamento (métodos ou funções).

- O que é programação procedural?

  A programação funcional é um paradigma de programação que se concentra na execução sequencial de procedimentos ou rotinas, também chamados de funções ou subprogramas. O foco principal está em como o programa é executado e quais passos são seguidos para se alcançar um determinado resultado.

- O que é programação funcional?

  A programação funcional é um paradigma de programação que se concentra na avaliação de expressões e na aplicação de funções matemáticas. Ela trata a computação como a avaliação de funções e evita o uso de estados mutáveis e dados compartilhados

- Qual a diferença entre programação orientada a objetos (OOP) e programação procedural?

  Na programação procedural, o foco está nas funções e no fluxo de execução, enquanto na POO, o foco está nos objetos e na interação entre eles.

- Qual a diferença entre programação orientada a objetos (OOP) e programação funcional?

  A programação orientada a objetos concentra-se em "objetos", seus dados (atributos ou propriedades) e comportamento (métodos ou funções) enquanto a programação funcional evita estados mutáveis e se concentra na aplicação de funções puras.

- Qual as quatro principais vantagens da programação orientada a objetos (OOP)?

  - Modularidade;
  - Reusabilidade ou Reuso de Código;
  - Facilidade de Manutenção;
  - Abstração.

- Dentro de OOP, o que é Modularidade?

  Modularidade consiste em dividir o seu software em partes menores (módulos) que podem ser desenvolvidos, testados, feito manutenção e reutilizados de forma independente.

- Dentro de OOP, o que é Reusabilidade ou Reuso de Código;?

  Módulos de um programa podem ser reutilizadas em diferentes partes do mesmo programa ou em diferentes programas, economizando tempo e esforço.

- Dentro de OOP, o que é Facilidade de Manutenção;?

  Como o código é organizado em módulos com propósitos específicos as mudanças/manutenção em um módulo têm menos probabilidade de afetar outras partes do sistema.

- Dentro de OOP, o que é Abstração?

  A OOP possibilita criar abstrações que mascaram a complexidade interna dos objetos, expondo apenas o que é necessário para interagir com eles. Isso torna o software mais fácil de se usar e entender.

- Dentro de OOP, o que é uma classe?

  Uma classe é a base para a criação de objetos em OOP. Ela fornece a estrutura necessária para criar e manipular objetos, encapsulando dados e comportamentos relacionados.

- Dentro de OOP, o que é uma objeto?

  Um objeto é uma instância de uma classe que possui estado (definido pelos dados em atributos ou propriedades), comportamento (métodos ou funções) e identidade (objetos são diferenciáveis entre si). Ele é criado a partir da classe e pode interagir com outros objetos e o ambiente de acordo com a estrutura e as funcionalidades definidas pela classe.

- Dentro de OOP, o que é uma objeto?

  Atributos são as variáveis ou propriedades que definem o estado de um objeto. Eles armazenam informações sobre o objeto e podem ser usados para representar características ou propriedades do mesmo. Quais atributos um objeto deve/pode possuir é definido pela sua classe.

- Como declarar uma classe em Python?

  Usando `class` como em

  ```python
  class Carro():
  	pass
  	## Atributos e métodos da classe
  ```

- Qual o método construtor de classes em Python?

  É o método especial `__init__`. Exemplo

  ```python
  class Carro():
  	def __init__(self, marca, qnt_portas: int, cor):
  		self.marca = marca
  		self.qnt_portas = qnt_portas
  		self.cor = cor
  ```

- Como instanciar um objeto em Python?

  Deve se criar uma instancia de uma classe.

  ```python
  # Def classe
  class Carro():
  	def __init__(self, marca, qnt_portas: int, cor):
  		self.marca = marca
  		self.qnt_portas = qnt_portas
  		self.cor = cor
  # Criação da instancia
  ntt_carro = Carro("Fiar Argo", "4", "Cinza")
  ```

- Dentro de OOP, o que é uma método?

  Métodos são funções associadas a uma classe, eles definem os comportamentos dos objetos criados a partir dessa classe. Eles podem manipular, consultar, retornar, etc. os atributos de um objeto.

- Por que o método construtor **init** é especial em um classe em Python?

  O método construtor é automaticamente invocado sempre que uma nova instancia da classe é criada. É esse método que inicializa o estado inicial do objeto segundo o que foi definido na classe.

- Quando começamos a escrever uma classe em Python não devemos esquecer de passar o keyword `self` dentro dos parâmetros do método construtor **init**. Ele que é responsável por referenciar o próprio objeto quando a instancia é criada.

- Como devemos referenciar uma variável interna de uma classe?

  Devemos usar o keyword self para chamar a variável interna da classe. Exemplo:

  ```python
  # Def classe
  class Carro():
  	def __init__(self, marca, qnt_portas: int, cor):
  		self.marca = marca
  		self.qnt_portas = qnt_portas
  		self.cor = cor

  	def descrever(self):
  		return f"A marca do carro é {self.marca} de cor {self.cor} e possui {self.qnt_portas} portas"
  ```

- Dentro de OOP, o que é o conceito de Encapsulamento?

  Esse conceito permite proteger e controlar o acesso ao estado interno do objeto. Por exemplo, se temos uma classe carro que possui um atributo velocidade e com métodos frear e acelerar. Esse métodos são responsáveis por modificar o atributo velocidade dentro do que é esperado do comportamento da classe de modo que não precisamos nos preocupar em como isso irá ocorrer quando quisermos executar um desses métodos. Além disso, é possível que o método possua limitações esperadas como velocidade máxima.

- Dentro de OOP, o que é o conceito de Abstração?

  Esse conceito permite construir níveis de “entendimento” para descrever comportamentos complexos dentro de um programa. Por exemplo, podemos criar uma classe motor de carro onde definimos uma aceleração máxima e depois criar uma classe carro que herda esse comportamento. Essa classe carro pode usar essa informação em métodos como acelerar além de poder possuir outros métodos e atributos únicos do carro como um todo (como cor). Assim, cada parte do código fica organizado e no seu devido nível de abstração.

- Dentro de OOP, o que é o conceito de Herança?

  Esse conceito pode ser definido como o reaproveitamento de propriedades (atributos e métodos) já definidas em outras classes. Isso permite abstrair e organizar as classes. Uma classe funcionário pode ser usada para criar as subclasses gerente, vendedor, etc.

- Dentro de OOP, o que é o conceito de Polimorfismo?

  Esse conceito está ligado a adequação de comportamentos comuns a varias classes para o seu uso especifico. Isso é, mesmo que duas classes possuam um método (por exemplo pagamento) podemos modificar esse método dentro de cada subclasse para adequar ao seu funcionamento (por exemplo pagamento com crédito, debito ou pix).

- Quais os três tipos de atributos de visibilidade em OOP?

  - Public: Atributos e métodos que podem ser invocados, acessados e modificados de qualquer lugar.
  - Private: Atributos e métodos que só podem ser invocados, acessados e modificados pelo seu próprio objeto.
  - Protected: Atributos e métodos que só podem ser invocados, acessados e modificados por classes herdeiras (filhas ou subclasses).

- Qual a convenção para uma propriedade ou método privado em Python?
  Colocar dois underlines (`__`) antes do nome do propriedade ou método.

- O que o seguinte método faz dentro dessa classe?

  ```python
  # Def classe
  class Carro():
  	def __init__(self, marca, qnt_portas: int, cor):
  		self.marca = marca
  		self.qnt_portas = qnt_portas
  		self.cor = cor

  	def descrever(self):
  		return f"A marca do carro é {self.marca} de cor {self.cor} e possui {self.qnt_portas} portas"
  ```

  Ele descrever o carro usando as informações do objeto. Por exemplo:

  ```python
  >>> ntt_carro = Carro("Fiar Argo", "4", "Cinza")
  >>> print(ntt_carro.descrever())
  "A marca do carro é Fiar Argo de cor Cinza e possui 4 portas"
  ```

- O que o seguinte método faz dentro dessa classe?

  ```python
  # Def classe
  class Carro():
  	def __init__(self, marca, qnt_portas: int, cor):
  		self.marca = marca
  		self.qnt_portas = qnt_portas
  		self.cor = cor

  	def verificar_qnt_portas(self,qnt_portas_comparativa):
  		if self.qnt_portas >= qnt_portas_comparativa:
  			return f"O carro possui mais, ou igual, do que {qnt_portas_comparativa} portas."
  		else:
  			return f"O carro não possui no minimo {qnt_portas_comparativa} portas."
  ```

  Ele utiliza a propriedade do objeto qnt_portas e o input do método para retornar uma mensagem indicando se o carro possui ou não esse número mínimo de portas.

  ```python
  >>> ntt_carro = Carro("Fiar Argo", 4, "Cinza")
  >>> print(ntt_carro.verificar_qnt_portas(2))
  "O carro possui mais, ou igual, do que 2 portas."
  ```

- Descreve a herança do código a seguir:

  ```python
  class Funcionario:
      daf __init__(self, nome, idade):
          self.nome = nome
          se1f.idade = idade

  class Setor:
      def __inft__(self, departamento):
          self.departamento= departamento

  class Diretor(Funcionario, Setor):
      def __init__(self, nome, idade, departamento, nivel):
          Funcionario.__init__(self, nome, idade)
          Setor.__init__(self, departanento)
          self.nivel = nivel
  ```

  Aqui temos a criação de duas classes simples (Funcionario e Setor) e a criação de uma classe Direto que herda as propriedades dessas duas classes.

- Qual o output 1 e 2?

  ```python
  class Passaro:
      def Yoar(self):
          return "Vando"

  class pinguin(Passaro):
      def Voar(self):
          return "Pinguin não podem voar, eles nadam!"

  passaro= Passaro()
  pinguin= Pinguin()
  print(passaro1.Voar()) # 1
  print(pinguim1.voar()) # 2
  ```

  Output 1: “Voando”
  
  Output 2: "Pinguin não podem voar, eles nadam!
