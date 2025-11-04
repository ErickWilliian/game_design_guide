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
      Debug.Log("Nome do jogador", nomePlayer);
    }


    void Update()
    {
        
    }
}

```


## Métodos com Retorno

Eles são diferentes do `void Start()` e o `void Update()` esses dois nao retornam nada pois começam com a diretiva `void`, ou seja que eles não tem retorno, no C# e linguagens fortemente tipadas você precisa indicar qual é o tipo de retorno que as funções vão ter, por exemplo se a função vai retornar um número tu deve colocar o `int` antes de nomear a função, por exemplo `int retornaNumero()`


Você pode passar parâmetros para as funções que são variáveis que sao recebidas nas chamadas das função

```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
    void Start()
    {
      // e aqui na chamada eu passo os valores para os param
      somaNumeros(1, 2);
    }

    void Update()
    { 
    }

    // aqui eu faço a definição da minha função com dois param
    // e retorno eles
    int somaNumeros(int a, int b){
      return a + b
    }
}

```


## Contador, Incremento, Decremento e Contador de tempo

```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
  int numero;
  float tempo;

    void Start()
    {
      // Incremento
      numero = numero + 1;
      numero = numero - 1;
    }

    void Update()
    { 
      // Contagem de tempo na unity
      tempo = tempo + Time.deltaTime;
    }

}

```

## Arrays / Vetores


```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
  int[] numero;

    void Start()
    {

    }

    void Update()
    { 

    }

}

```

## Listas e coleções 


```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
  List<int> numeros = new List<int>();

    void Start()
    {
      // Para adicionar em uma lista
      numeros.Add(2);

      numeros[1] = 4;

      // Para remover um item pela posição passada
      numeros.RemoveAt(1)

      // Para organizar a lista
      numeros.Sort();
    }

    void Update()
    { 

    }

}

```


## COLEÇÃO DICTIONARY / DICIONARIOS

```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
  Dictionary<string, string> viloes = new Dictionary<string, string>();

    void Start()
    {
      viloes.Add("ceifador","vilão da primeira fase" + "altura:180cm")
    }

    void Update()
    { 

    }

}

```

## Classes

```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
    void Start()
    {
     
    }

    void Update()
    { 

    }

}
class Vampiros{
  int força, velocidade;
  
  void ataque(){

  }
}
```


## Herança

Classes podem herdar caracteristicas de outras classes por exemplo a minha classe vampiros herdam da classe inimigos e ai ele sempre vai ter as funções e coisas basicas de inimigos

```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
    void Start()
    {
     
    }

    void Update()
    { 

    }

}
class Inimigos{
  int força, velocidade;
    
  void ataque(){

  }
}


class Vampiros : Inimigos{
  
}
```

E essas heranças podem fazer cascata ou seja se em algum momento eu queira criar um novo inimigo por exemplo "ReiVampiro" e fazer ele herdar da classe vampiros ele também vai receber da classe inimigos e assim por diante

Existe um detalhe muito importante que as classes que recebem herança de outras classes so podem pegar funções e variaveis se elas estiverem como public

```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{
    void Start()
    {
     
    }

    void Update()
    { 

    }

}
class Inimigos{
  public int vida = 100;          // pode ser acessada por qualquer classe
  private int força = 50;         // só a classe Inimigo vê
  protected int velocidade = 10;  // visível em subclasses

  // Pode ser usada em outras classes  
  public void ataque(){

  }

  // essa função nao pode ser herdada
  private void teste(){

  }
}


class Vampiros : Inimigos{
  
}
```


## Objetos e Instâncias de classes

```c#
using UnityEngine;

public class Variaveis : MonoBehaviour
{

    Vampiros Dracula = new Vampiros();
    void Start()
    {
      Dracula.força = 100
      Dracula.velocidade = 100
    }

    void Update()
    { 

    }

}
class Inimigos{
  public int vida = 100;         
  public int força = 50;         
  public int velocidade = 10;  
 
  public void ataque(){

  }

  private void teste(){

  }
}


class Vampiros : Inimigos{
  
}
```