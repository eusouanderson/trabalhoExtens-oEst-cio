## Encapsulamento em Java

**Encapsulamento** é um dos pilares da programação orientada a objetos. Ele se refere ao conceito de agrupar dados (atributos) e métodos (funções) que operam sobre esses dados em uma única unidade, chamada de classe. Além disso, encapsulamento protege o estado interno do objeto de acesso direto e não autorizado, expondo apenas os métodos necessários para a interação com o objeto. Isso é feito utilizando modificadores de acesso.

### Conceitos Principais

- **Atributos Privados:** Os atributos de uma classe são declarados como `private`, o que impede acesso direto de fora da classe.
- **Métodos Públicos:** Métodos `public` são fornecidos para acessar e modificar os atributos privados. Estes métodos são chamados de *getters* e *setters*.

### Exemplo de Encapsulamento

Aqui está um exemplo de como encapsulamento pode ser implementado em Java:

```java
public class Pessoa {
    // Atributos privados
    private String nome;
    private int idade;

    // Método público para acessar o nome
    public String getNome() {
        return nome;
    }

    // Método público para definir o nome
    public void setNome(String nome) {
        this.nome = nome;
    }

    // Método público para acessar a idade
    public int getIdade() {
        return idade;
    }

    // Método público para definir a idade
    public void setIdade(int idade) {
        if (idade > 0) {
            this.idade = idade;
        }
    }
}
```

## Explicação do Código
### Atributos Privados:

```java

private String nome;
private int idade;

```
#### Os atributos nome e idade são declarados como private, o que significa que eles não podem ser acessados diretamente fora da classe Pessoa.

### Métodos Públicos:
```java
public String getNome() e public void setNome(String nome) são métodos para acessar e modificar o atributo nome.
public int getIdade() e public void setIdade(int idade) são métodos para acessar e modificar o atributo idade.
```

#### Os métodos getNome() e getIdade() permitem que outras partes do código obtenham o valor dos atributos, enquanto os métodos setNome(String nome) e setIdade(int idade) permitem que os atributos sejam modificados. No caso do método setIdade(int idade), há uma verificação para garantir que a idade seja positiva antes de ser definida.

## Vantagens do Encapsulamento

* Proteção de Dados: Impede acesso e modificação indesejada dos atributos internos.
* Facilidade de Manutenção: Permite alterar a implementação interna sem afetar o código que usa a classe.
* Controle: Permite validar os dados antes de modificá-los, como demonstrado no método setIdade.

#### O encapsulamento é essencial para criar classes que são fáceis de usar e seguras, mantendo o controle sobre como os dados são acessados e modificados.


Voltar a [Abstração](Abstração.md) Ir para [Herança](Herança.md)

