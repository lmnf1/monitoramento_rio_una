# Sistema de Monitoramento do Rio Una — Palmares

## Sobre o projeto

Este projeto consiste em um software simples de **monitoramento preventivo do Rio Una**, desenvolvido pensando no contexto de **Palmares**.

O sistema tem como objetivo acompanhar, de forma simulada, o nível do rio e informar sua situação atual, podendo indicar se o nível está **normal, em atenção ou em alerta**.

A proposta busca contribuir para o acompanhamento das condições do Rio Una e, ao mesmo tempo, demonstrar a utilização de ferramentas de **Git e GitHub**, com organização de commits, branches, Pull Requests, revisões e releases.

**Objetivos:**

* Acompanhar, de forma simulada, o nível do Rio Una e informar a situação atual.
* Servir de projeto educacional para praticar Git e GitHub, com branches, commits claros, Pull Requests, revisões e release.

> **Protótipo educacional.** Este sistema ainda **não possui integração com sensores reais do Rio Una**. Os valores são simulados ou registrados manualmente, **não** representam medição oficial e **não** devem ser usados como orientação de risco ou de evacuação.

## Problema local

O projeto está relacionado ao monitoramento do **Rio Una em Palmares**, permitindo acompanhar alterações no nível da água.

A solução apresenta informações como:

* Nível atual do rio;
* Situação: normal, atenção ou alerta;
* Histórico das medições;
* Área de avisos;
* Local monitorado (Rio Una, em Palmares).

Os dados utilizados são **simulados ou registrados manualmente**, não sendo necessária a utilização de sensores reais.

## Justificativa do projeto

O desenvolvimento deste sistema se justifica pela importância do monitoramento do Rio Una em Palmares, Pernambuco. A elevação do nível da água pode representar riscos para as áreas próximas ao rio, especialmente durante períodos de chuvas intensas.

O projeto busca demonstrar como a tecnologia pode contribuir para a conscientização ambiental e para a compreensão da importância do acompanhamento do nível dos rios. O sistema possui finalidade educativa e utiliza dados simulados, não substituindo medições reais ou alertas oficiais.

## Funcionalidades

* Exibição do nível atual e da situação (Normal, Atenção ou Alerta).
* **Registro manual de medições.**
* Histórico das medições, **guardado no navegador**: ele continua depois de recarregar a página, mas fica apenas no computador e no navegador usados.
* Gráfico do nível com **escala dinâmica**, que se ajusta aos valores registrados.
* **Exportação dos dados em CSV.**
* Área de avisos conforme a situação.
* **Melhorias de interface, responsividade e acessibilidade**: o layout se adapta a diferentes tamanhos de tela.
* Modo claro e modo escuro.

## Tecnologias utilizadas

* HTML, CSS e JavaScript puros, sem bibliotecas externas.
* Armazenamento do navegador (localStorage) para guardar o histórico.
* Gráfico desenhado em SVG.
* Git e GitHub para o versionamento; Git Bash e VS Code no desenvolvimento.

## Como executar

Não é preciso instalar nada. Você só precisa de um navegador moderno (Chrome, Edge ou Firefox).

1. Clone o repositório (ou baixe o ZIP pelo botão **Code** do GitHub):
   ```bash
   git clone https://github.com/lmnf1/monitoramento-rio-una.git
   ```
2. Entre na pasta do código:
   ```bash
   cd monitoramento-rio-una/monitoramento-rio-una
   ```
3. Abra o arquivo `index.html` no navegador (clique duas vezes nele).
4. Registre medições e acompanhe o nível, a situação, o histórico e o gráfico.
5. Use a opção de exportação para baixar os dados em CSV.

## Evolução das versões

* **v1.0.0** — Primeira versão estável do sistema de monitoramento do Rio Una.
* **Versão atual (nova)** — acrescenta o registro manual de medições, o histórico guardado no navegador, a escala dinâmica do gráfico, a exportação em CSV e melhorias de interface, responsividade e acessibilidade.

As versões finais são marcadas com tag/release na aba **Releases** do GitHub.

## Processo de versionamento

O projeto utiliza Git e GitHub para controlar as alterações do código. As funcionalidades são desenvolvidas em branches separadas e integradas à branch principal após revisão por Pull Request.

### Padrões de contribuição

Para contribuir com o projeto, é necessário manter a organização do repositório.

As contribuições devem seguir estas regras:

* Criar uma **branch** para cada alteração;
* Fazer commits claros e relacionados à alteração realizada, começando com um verbo (por exemplo: "Adiciona exportação dos dados em CSV");
* Revisar as alterações antes do merge;
* Utilizar **Pull Requests** para integrar as alterações;
* Corrigir possíveis conflitos antes da integração;
* Manter o código e a documentação organizados.

### Política de ramificação

O projeto utiliza branches para organizar o desenvolvimento e evitar alterações diretamente na versão principal.

Cada integrante deve trabalhar em sua própria branch para desenvolver suas tarefas. Depois, as alterações devem ser enviadas por meio de **Pull Request**, passando por revisão antes de serem integradas à branch principal.

Essa organização permite acompanhar a evolução do projeto e manter um histórico de versionamento organizado.

### Como ver o histórico e a contribuição de cada integrante

No GitHub, use a aba **Commits**, a aba **Pull requests** e **Insights > Contributors**. No terminal:

```bash
git log --oneline --graph --all
git shortlog -sn --all
```

## Divisão das funções do grupo

| Integrante | Função                     | O que faz                                                                                               |
|------------|----------------------------|---------------------------------------------------------------------------------------------------------|
| Lívia      | Desenvolvimento do sistema | Implementa as funcionalidades, testa o fluxo principal e registra como executar o programa.             |
| Isabel     | README e documentação      | Explica o problema local, as funcionalidades, as tecnologias, a execução, as versões e o versionamento. |
| Vinícius   | Git e versionamento        | Cria as branches, organiza commits e Pull Requests, pede revisões e cria a tag/release.                 |
| Isabella   | Organização e apresentação | Organiza o trabalho do grupo e cuida da apresentação final.                                             |

## Projeto de inspiração

* Projeto original: https://github.com/Honey-git/FloodMonitor
* Nosso fork: https://github.com/isabel684755/FloodMonitor
* O que aproveitamos: a forma de documentar os níveis de risco, explicando a regra de cada nível (Safe, Warning e Danger no FloodMonitor), e a organização do README em seções.
* Diferença: o FloodMonitor usa sensor físico e validação estatística; o nosso sistema é um protótipo educacional, sem sensores reais.