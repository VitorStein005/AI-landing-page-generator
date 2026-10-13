# AI Landing Page Generator

Gerador de landing pages com inteligência artificial, desenvolvido como
projeto prático durante a imersão **Missão Programação com IA do Zero**,
do DevClub.

## Sobre o projeto

O AI Landing Page Generator permite informar o tipo de negócio desejado
--- por exemplo, uma cafeteria, um mercado ou outro empreendimento --- e
solicitar à inteligência artificial a criação de uma landing page
personalizada.

A aplicação exibe o código gerado e uma prévia da página no navegador.

## Funcionalidades

-   Recebe uma descrição ou tipo de negócio informado pelo usuário.
-   Envia a solicitação para a API da Groq.
-   Gera o conteúdo de uma landing page em HTML e CSS.
-   Exibe o código retornado pela IA.
-   Apresenta uma prévia da página gerada.

## Tecnologias utilizadas

-   **HTML5** --- estrutura da interface.
-   **CSS3** --- estilização da interface.
-   **JavaScript** --- lógica da aplicação e chamada à API.
-   **Groq API** --- geração de conteúdo com inteligência artificial.

## Arquivos do projeto

-   `index.html` --- estrutura da aplicação.
-   `style.css` --- estilos da interface.
-   `scripts.js` --- lógica de geração e integração com a API da Groq.

## Como obter uma chave da Groq

Para utilizar a funcionalidade de geração, você precisa de uma chave de
API própria.

1.  Acesse a página oficial: [GroqCloud --- API
    Keys](https://console.groq.com/keys).
2.  Entre na sua conta GroqCloud. Se ainda não tiver uma conta, siga o
    processo de cadastro.
3.  Na área de API Keys, crie uma nova chave seguindo as opções
    apresentadas na plataforma.
4.  Copie e guarde a chave em local seguro. Não a publique nem a
    compartilhe.

A interface do GroqCloud pode mudar com o tempo; siga as opções exibidas
na sua conta.

## Como configurar a chave

1.  Baixe ou clone este repositório para o computador.

2.  Abra a pasta do projeto no Visual Studio Code.

3.  Abra o arquivo `scripts.js`.

4.  Localize o cabeçalho de autenticação dentro da chamada `fetch`:

    ``` javascript
    "Authorization": "Key"
    ```

5.  Substitua o valor pelo formato abaixo, colocando sua chave no lugar
    de `SUA_CHAVE_DA_GROQ`:

    ``` javascript
    "Authorization": "Bearer SUA_CHAVE_DA_GROQ"
    ```

6.  Salve o arquivo.

**Importante:** mantenha a palavra `Bearer`, o espaço e a chave no mesmo
valor da propriedade `Authorization`. Não compartilhe o arquivo com sua
chave pessoal preenchida.

## Como executar

1.  Abra a pasta do projeto no Visual Studio Code.
2.  Abra o arquivo `index.html` no navegador. Você pode usar o Chrome ou
    uma ferramenta de pré-visualização local.
3.  Digite uma descrição do negócio no campo de texto.
4.  Clique em **Gerar** e aguarde a resposta da API.

A geração depende de uma chave válida e do acesso à API da Groq. Se
houver erro, confira a chave, o cabeçalho de autenticação, a conexão com
a internet e a disponibilidade do modelo configurado no arquivo
`scripts.js`.

## Segurança da chave da API

Este projeto, na versão atual, faz a chamada à Groq diretamente pelo
JavaScript executado no navegador. Isso significa que a chave usada no
arquivo pode ser visualizada por outras pessoas que tenham acesso ao
código ou inspecionem as requisições do navegador.

-   Não coloque uma chave pessoal em um repositório público.
-   Não publique capturas de tela que mostrem sua chave.
-   Para experimentar localmente, use sua própria chave e evite
    compartilhar o arquivo configurado.
-   Para publicar a aplicação para outras pessoas, o recomendado é mover
    a chamada à API para um backend e manter a chave em uma variável de
    ambiente no servidor.

## Aprendizados

Este projeto foi uma oportunidade de praticar HTML, CSS e JavaScript,
além de explorar a integração de uma aplicação web com uma API de
inteligência artificial.

## Possíveis melhorias futuras

-   Criar um backend para proteger a chave da API.
-   Adicionar mensagens de carregamento e tratamento de erros.
-   Oferecer mais opções de personalização para a landing page gerada.
-   Melhorar a experiência de uso e a acessibilidade da interface.

## Autor

Projeto desenvolvido por Victor Stenda Silva como parte de sua jornada
de aprendizado em desenvolvimento web.
