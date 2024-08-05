# Polimorfismo em Java

**Polimorfismo** é a capacidade de um objeto assumir várias formas, permitindo que uma única interface seja usada para representar diferentes tipos de objetos. Em Java, o polimorfismo pode ser alcançado de duas maneiras principais: **sobrecarga de métodos** e **sobrescrição de métodos**.

## Sobrecarga de Métodos

**Sobrecarga de métodos** ocorre quando duas ou mais funções na mesma classe têm o mesmo nome, mas parâmetros diferentes (tipos, número ou ambos). A decisão sobre qual método chamar é feita em tempo de compilação com base nos argumentos fornecidos.

### Exemplo de Sobrecarga de Métodos

```java
// Classe que demonstra a sobrecarga de métodos
public class Calculadora {
    // Método para somar dois inteiros
    int soma(int a, int b) {
        return a + b;
    }

    // Método para somar dois números de ponto flutuante
    double soma(double a, double b) {
        return a + b;
    }
}

```
## Explicação do Código:

* Método soma(int a, int b): Este método soma dois números inteiros e retorna o resultado como um inteiro.

* Método soma(double a, double b): Este método soma dois números de ponto flutuante e retorna o resultado como um número de ponto flutuante.

#### A sobrecarga permite que você use o mesmo nome de método para operações semelhantes, mas com diferentes tipos de parâmetros.

### Sobrescrição de Métodos

#### Sobrescrição de métodos ocorre quando uma classe derivada fornece uma implementação específica de um método que já está definido na sua classe base. O método na classe derivada deve ter o mesmo nome, tipo de retorno e parâmetros que o método na classe base.

## Exemplo de Sobrescrição de Métodos
```java 
// Classe base
public class Animal {
    void emitirSom() {
        System.out.println("O animal faz um som.");
    }
}

// Classe derivada
public class Cachorro extends Animal {
    @Override
    void emitirSom() {
        System.out.println("O cachorro late.");
    }
}
```
## Explicação do Código:

#### Método emitirSom() na classe Animal: Este método é definido na classe base e fornece uma implementação genérica.

#### Método emitirSom() na classe Cachorro: Este método sobrescreve a implementação do método da classe base, fornecendo uma implementação específica para o comportamento de um cachorro.

* Conclusão

#### O polimorfismo é uma característica fundamental da programação orientada a objetos que permite que objetos sejam manipulados de formas diferentes dependendo de seu tipo real. Com a sobrecarga de métodos, você pode definir múltiplos métodos com o mesmo nome, mas com diferentes parâmetros. Com a sobrescrição de métodos, você pode alterar o comportamento dos métodos herdados para se adequar às necessidades da classe derivada.


Voltar a [Herança](Herança.md) Ir para [Objeto](Objeto.md)