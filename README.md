# uml-class-java
```mermaid
classDiagram
    class ReprodutorMusical
    <<interface>> ReprodutorMusical
        ReprodutorMusical:tocar()
        ReprodutorMusical:pausar()
        ReprodutorMusical:selecionarMusica(String musica)

    
    class AparelhoTelefonico
    <<interface>> AparelhoTelefonico
        AparelhoTelefonico:ligar(String numero)
        AparelhoTelefonico:atender()
        AparelhoTelefonico:iniciarCorreioVoz()

    class NavegadorInternet
    <<interface>> NavegadorInternet
        NavegadorInternet:exibirPagina(String url)
        NavegadorInternet:adicionarNovaAba()
        NavegadorInternet:atualizarPagina()

    class Smartphone {
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

    ReprodutorMusical <|.. Smartphone
    AparelhoTelefonico <|.. Smartphone
    NavegadorInternet <|.. Smartphone
