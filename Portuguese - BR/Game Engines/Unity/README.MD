# C# para Unity


## Criando Variáveis:

- Espaços na memoria para guardar valores
- No C# precisamos sempre indicar o valor das variáveis e elas consistem em 
  - int > para valores numéricos inteiros
  - float > para números com vírgula e precisa sempre colocar um "f" no fim e a vírgula no C# é o "."
  - bool > valores booleanos são valores de Verdadeiro (true) ou Falso (false)
  - string > para tipo de textos
- Sempre lembre de quando terminar de escrever uma linha colocar ponto e vírgula
```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
    // Podemos declarar assim as variáveis 
    // Também podemos colocar múltiplas variáveis na mesma linha
    int vidaPlayer = 10, forca = 20;
    float jumpForce = 3.0f;
    bool mortePlayer = false;
    string nomePlayer = "Erick";

    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        
    }
}

```

## Métodos "void Start" e "void Update"

Métodos ou funções são blocos de códigos que podem ser reutilizados a qualquer momento chamando seu nome 

Por padrão a Unity ja cria essas duas funções

```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
    // Executa assim que o jogo começa ou o elemento renderizado na tela do jogo
    void Start()
    {
        // Para imprimir um texto no terminal voce usa print
        print("Teste 1234");
    }

    // Chamada a cada momento, ou seja a cada mudança de frame ele executa até o elemento sair da tela
    void Update()
    {
        
    }
}

```


## Variáveis Locais e Variáveis Globais

```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
    // Quando a variável estiver fora de funções ela é uma variável global
    // E sendo global ela pode ser acessada em qualquer lugar do código
    string variavelGlobal = "teste";

    void Start()
    {
      // Aqui ela é uma variável Local e so pode ser acessada dentro desta função
      string nomePlayer = "Erick ";
    }


    void Update()
    {
        
    }
}

```