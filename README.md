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

```mermaid
classDiagram
    ReprodutorMusical : tocar()
    ReprodutorMusical : pausar()
    ReprodutorMusical : selecionarMusica(String musica)

    AparelhoTelefonico : ligar(String numero)
    AparelhoTelefonico : atender()
    AparelhoTelefonico : iniciarCorreioVoz()

    NavegadorNaInternet : exibirPagina(String url)
    NavegadorNaInternet : adicionarNovaAba()
    NavegadorNaInternet : atualizarPagina()

    iPhone ..|> ReprodutorMusical
    iPhone ..|> AparelhoTelefonico
    iPhone ..|> NavegadorNaInternet
