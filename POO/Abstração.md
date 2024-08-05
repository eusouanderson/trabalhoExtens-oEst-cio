## Abstração em Java

**Abstração** é o processo de esconder a complexidade interna e exibir apenas as informações essenciais ao usuário. Em outras palavras, abstração permite que você se concentre no que um objeto faz, sem se preocupar com os detalhes de sua implementação. Isso é fundamental para reduzir a complexidade e aumentar a modularidade no desenvolvimento de software.

Em Java, a abstração pode ser implementada usando **classes abstratas** e **interfaces**. 

### Classes Abstratas

Uma **classe abstrata** é uma classe que não pode ser instanciada diretamente. Ela serve como uma base para outras classes e pode conter métodos abstratos (métodos sem implementação) que devem ser implementados pelas classes derivadas. Além disso, uma classe abstrata pode ter métodos concretos (com implementação).

**Exemplo de Classe Abstrata:**

```java
// Classe abstrata
public abstract class Forma {
    // Método abstrato (sem implementação)
    abstract void desenhar();
    
    // Método concreto (com implementação)
    public void mover() {
        System.out.println("Movendo a forma.");
    }
}
```
Voltar a [Introdução](Introdução.md) Ir para [Encapsulamento](Encapsulamento.md)