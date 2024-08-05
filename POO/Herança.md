## Herança em Java

**Herança** é um dos principais conceitos da programação orientada a objetos. Ela permite que você crie uma nova classe baseada em uma classe existente. A classe existente é chamada de **classe base** (ou classe pai), e a nova classe é chamada de **classe derivada** (ou classe filha). Herança permite que a classe derivada herde atributos e métodos da classe base, promovendo a reutilização de código e a criação de uma hierarquia de classes.

### Conceitos Principais

- **Classe Base:** A classe que fornece atributos e métodos para outras classes.
- **Classe Derivada:** A classe que herda atributos e métodos da classe base e pode adicionar ou sobrescrever comportamentos.

### Exemplo de Herança

Aqui está um exemplo que demonstra como a herança é usada em Java:

```java
// Classe base
public class Animal {
    // Método da classe base
    void emitirSom() {
        System.out.println("O animal faz um som.");
    }
}

// Classe derivada
public class Cachorro extends Animal {
    // Sobrescreve o método da classe base
    @Override
    void emitirSom() {
        System.out.println("O cachorro late.");
    }
}
```

## Explicação do Código

### Classe Base Animal:

* Define um método emitirSom() que imprime uma mensagem indicando que o animal faz um som.
* Esta classe serve como base para outras classes que representam tipos específicos de animais.
### Classe Derivada Cachorro:

* Estende a classe Animal usando a palavra-chave extends.
* Sobrescreve o método emitirSom() da classe base para fornecer uma implementação específica para um cachorro. Aqui, o método imprime uma mensagem indicando que o cachorro late.
### Vantagens da Herança
* Reutilização de Código: Permite que você reutilize código existente, evitando duplicação.
* Organização: Ajuda a organizar e estruturar o código de forma hierárquica.
* Extensibilidade: Facilita a adição de novos comportamentos ou características sem alterar o código existente.
## Conclusão
Herança é uma ferramenta poderosa que permite criar novas classes baseadas em classes existentes, promovendo a reutilização e a organização do código. Ela ajuda a construir uma hierarquia de classes que reflete relações do mundo real e pode simplificar a manutenção e a extensão do código.


Voltar a [Encapsulamento](Encapsulamento.md) Ir para [Polimorfismo](Polimorfismo.md)