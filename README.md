#  Sistema de Monitoramento do Rio Una — Palmares

##  Sobre o projeto

O **Sistema de Monitoramento do Rio Una** é um projeto educativo que tem como finalidade demonstrar o acompanhamento preventivo do nível do Rio Una, localizado na região de Palmares, Pernambuco.

O sistema utiliza dados simulados para apresentar o nível da água e classificar a situação do rio como **normal, atenção ou alerta**. Também propõe a apresentação do histórico das medições, avisos e informações sobre os pontos de monitoramento.

A proposta busca contribuir para o acompanhamento das condições do Rio Una e, ao mesmo tempo, demonstrar a utilização de ferramentas de **Git e GitHub**, com organização de commits, branches, Pull Requests, revisões e releases.

**Objetivos:**

* Acompanhar, de forma simulada, o nível do Rio Una e informar a situação atual.
* Servir de projeto educacional para praticar Git e GitHub, com branches, commits claros, Pull Requests, revisões e release.

> **Protótipo educacional.** Este sistema ainda **não possui integração com sensores reais do Rio Una**. Os valores são simulados ou registrados manualmente, **não** representam medição oficial e **não** devem ser usados como orientação de risco ou de evacuação.

##  Problema local

O Rio Una faz parte da realidade de Palmares, e as alterações no nível da água podem representar riscos para as áreas próximas, especialmente durante períodos de chuvas intensas.

Diante disso, o projeto propõe uma solução educativa para demonstrar como a tecnologia pode auxiliar no acompanhamento das condições de um rio e na conscientização sobre a prevenção de riscos ambientais.

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
* Histórico das últimas seis medições, **guardado no navegador**: ele continua depois de recarregar a página, mas fica apenas no computador e no navegador usados.
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
   git clone https://github.com/lmnf1/monitoramento_rio_una.git
   ```
2. Entre na pasta do código:
   ```bash
   cd monitoramento_rio_una
   ```
3. Abra o arquivo `index.html` no navegador (clique duas vezes nele).
4. Registre medições e acompanhe o nível, a situação, o histórico e o gráfico.
5. Use a opção de exportação para baixar os dados em CSV.

## Evolução das versões

* **v1.0.0** — Primeira versão estável do sistema de monitoramento do Rio Una.
* **v2.0.0** — acrescenta o registro manual de medições, o histórico guardado no navegador, a escala dinâmica do gráfico, a exportação em CSV e melhorias de interface, responsividade e acessibilidade.

As versões finais são marcadas com tag/release na aba **Releases** do GitHub.

## Processo de versionamento

O projeto utiliza Git e GitHub para controlar as alterações do código. As funcionalidades são desenvolvidas em branches separadas e integradas à branch principal após revisão por Pull Request.

### Padrões de contribuição

- Criar branches por tarefa, registrar commits claros e relacionar alterações às Issues.
- Revisar Pull Requests e resolver conflitos antes do merge.

### Política de ramificação

As alterações são integradas à branch main por Pull Request.

### Como ver o histórico e a contribuição de cada integrante

No GitHub, use a aba **Commits**, a aba **Pull requests** e **Insights > Contributors**. No terminal:

```bash
git log --oneline --graph --all
git shortlog -sn --all
```
## Aprendizados do projeto

O projeto possibilita praticar:

- Organização e documentação de um projeto de software;
- Uso de Git e GitHub;
- Criação e gerenciamento de Issues;
- Criação de branches e realização de commits;
- Revisão e integração de código por Pull Requests;
- Discussão sobre tecnologia e conscientização ambiental.

## Divisão das funções do grupo

| Integrante | Função                     | O que faz                                                                                               |
|------------|----------------------------|---------------------------------------------------------------------------------------------------------|
| Lívia      | Desenvolvimento do sistema | Implementa as funcionalidades, testa o fluxo principal e registra como executar o programa.             |
| Isabel     | README e documentação      | Explica o problema local, as funcionalidades, as tecnologias, a execução, as versões e o versionamento. |
| Isabella   | Organização e apresentação | Organiza o trabalho do grupo e cuida da apresentação final.                                             |
O projeto utiliza o Git para registrar as alterações e o GitHub para hospedar o repositório e facilitar o trabalho em equipe.

## Projeto de inspiração

* Projeto original: https://github.com/Honey-git/FloodMonitor
* Nosso fork: https://github.com/isabel684755/FloodMonitor
* O que aproveitamos: a forma de documentar os níveis de risco, explicando a regra de cada nível (Safe, Warning e Danger no FloodMonitor), e a organização do README em seções.
* Diferença: o FloodMonitor usa sensor físico e validação estatística; o nosso sistema é um protótipo educacional, sem sensores reais.
---

**Projeto educativo desenvolvido para estudar programação, versionamento e monitoramento ambiental no contexto de Palmares, Pernambuco.**
