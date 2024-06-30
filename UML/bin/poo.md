classDiagram
    IPhone <|-- ReprodutorMusical
    IPhone <|-- AparelhoTelefonico
    IPhone <|-- NavegadorInternet
     class ReprodutorMusical{
      -Musica[] musicas
      +tocar() void
      +pausar() void
      +selecionarMusica() void
    }
    class AparelhoTelefonico{
      -Contato[] contatos
      -redeMovelDisponivel() Boolean
      +ligar() void
      +atender() void
      +iniciarCorreioVoz() void
    }
    class NavegadorInternet{
      -conexaoComInternet() Boolean
      +exibirPagina() void
      +adicionarNovaAba() void
      +atualizarPagina() void
    }