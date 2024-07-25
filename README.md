# Desafio de POO - iPhone

## Contexto

Neste desafio, foi criada a modelagem e diagramação UML do componente iPhone, abrangendo suas funcionalidades como Reprodutor Musical, Aparelho Telefônico e Navegador na Internet.

## Funcionalidades

- **Reprodutor Musical**
  - `tocar()`
  - `pausar()`
  - `selecionarMusica(String musica)`

- **Aparelho Telefônico**
  - `ligar(String numero)`
  - `atender()`
  - `iniciarCorreioVoz()`

- **Navegador na Internet**
  - `exibirPagina(String url)`
  - `adicionarNovaAba()`
  - `atualizarPagina()`

## Diagrama UML

classDiagram
    class iPhone {
        -ReprodutorMusical reprodutorMusical
        -AparelhoTelefonico aparelhoTelefonico
        -NavegadorNaInternet navegadorNaInternet
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }

    class ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }

    class AparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }

    class NavegadorNaInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }
    
    iPhone o-- ReprodutorMusical
    iPhone o-- AparelhoTelefonico
    iPhone o-- NavegadorNaInternet

