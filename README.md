#  Sistema de Monitoramento do Rio Una — Palmares

##  Sobre o projeto

O **Sistema de Monitoramento do Rio Una** é um projeto educativo que tem como finalidade demonstrar o acompanhamento preventivo do nível do Rio Una, localizado na região de Palmares, Pernambuco.

O sistema utiliza dados simulados para apresentar o nível da água e classificar a situação do rio como **normal, atenção ou alerta**. Também propõe a apresentação do histórico das medições, avisos e informações sobre os pontos de monitoramento.

A proposta busca contribuir para o acompanhamento das condições do Rio Una e, ao mesmo tempo, demonstrar a utilização de ferramentas de **Git e GitHub**, com organização de commits, branches, Pull Requests, revisões e releases.

**Objetivos:**

* Acompanhar, de forma simulada, o nível do Rio Una e informar a situação atual.
* Servir de projeto educacional para praticar Git e GitHub, com branches, commits claros, Pull Requests, revisões e release.

> **Protótipo educacional.** Este sistema ainda **não possui integração com sensores reais do Rio Una**. Os valores são simulados ou registrados manualmente, **não** representam medição oficial e **não** devem ser usados como orientação de risco ou de evacuação.
Além da proposta ambiental, o projeto permite praticar o uso do Git e do GitHub, aplicando conceitos de versionamento, branches, commits, Issues e Pull Requests.

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
**Importante:** o sistema utiliza dados simulados e não substitui medições reais, sistemas oficiais de monitoramento ou alertas emitidos pelos órgãos responsáveis.

##  Justificativa do projeto

O desenvolvimento deste projeto se justifica pela importância de discutir o monitoramento dos rios e a prevenção de riscos ambientais em Palmares. A utilização da tecnologia pode contribuir para a compreensão das mudanças no nível da água e para a conscientização da população sobre a importância do acompanhamento dos rios.

A proposta também permite que os integrantes da equipe desenvolvam conhecimentos de programação, documentação e trabalho colaborativo por meio de ferramentas de versionamento.

##  Objetivos do projeto

### Objetivo geral

Desenvolver um sistema educativo de monitoramento preventivo simulado do Rio Una, demonstrando como a tecnologia pode auxiliar no acompanhamento do nível da água.

### Objetivos específicos

- Apresentar o nível atual do rio por meio de dados simulados;
- Classificar a situação do rio como normal, atenção ou alerta;
- Demonstrar o histórico das medições;
- Organizar avisos relacionados ao monitoramento;
- Apresentar informações sobre os pontos de monitoramento;
- Aplicar boas práticas de colaboração e versionamento com Git e GitHub.

* Criar uma **branch** para cada alteração;
* Fazer commits claros e relacionados à alteração realizada, começando com um verbo (por exemplo: "Adiciona exportação dos dados em CSV");
* Revisar as alterações antes do merge;
* Utilizar **Pull Requests** para integrar as alterações;
* Corrigir possíveis conflitos antes da integração;
* Manter o código e a documentação organizados.

### Política de ramificação
##  Funcionalidades previstas

- **Nível do rio:** apresentação do nível da água.
- **Classificação:** indicação das situações normal, atenção ou alerta.
- **Histórico:** organização das medições realizadas.
- **Avisos:** apresentação de mensagens relacionadas ao estado do rio.
- **Pontos de monitoramento:** exibição de informações sobre os locais acompanhados.

*As funcionalidades dependem da implementação disponível na versão atual do sistema.*

##  Tecnologias e ferramentas

- **Git:** controle de versões do projeto.
- **GitHub:** hospedagem do repositório e colaboração entre os integrantes.
- **Linguagens e tecnologias do sistema:** devem ser informadas conforme as ferramentas realmente utilizadas no desenvolvimento.

##  Como utilizar

1. Clone ou baixe este repositório.
2. Abra a pasta do projeto no computador.
3. Consulte os arquivos e as instruções de execução disponíveis.
4. Execute o sistema conforme as orientações do projeto.
5. Visualize as informações de monitoramento utilizando os dados simulados.

**Observação:** as instruções específicas de instalação e execução devem ser atualizadas conforme a implementação do sistema.

##  Padrões de contribuição

Para manter o projeto organizado, os integrantes devem seguir estas práticas:

- Criar uma branch para cada tarefa;
- Utilizar commits com mensagens claras e descritivas;
- Relacionar as alterações às Issues correspondentes;
- Abrir Pull Requests para apresentar as mudanças;
- Revisar as alterações antes da integração;
- Resolver possíveis conflitos;
- Manter o código e a documentação atualizados.

##  Política de ramificação

O desenvolvimento é organizado em branches separadas, evitando alterações diretas na branch principal.

Cada integrante deve criar uma branch para sua tarefa, realizar os commits necessários e enviar as alterações por meio de um Pull Request. Após a revisão e a aprovação, as alterações poderão ser integradas à branch principal.

### Como ver o histórico e a contribuição de cada integrante

No GitHub, use a aba **Commits**, a aba **Pull requests** e **Insights > Contributors**. No terminal:

```bash
git log --oneline --graph --all
git shortlog -sn --all
```
- **Lívia:** desenvolvimento e funcionalidades do sistema.
- **Isabel:** README e documentação.
- **Vinícius:** Git e versionamento.
- **Isabella:** organização e apresentação.

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
| Vinícius   | Git e versionamento        | Cria as branches, organiza commits e Pull Requests, pede revisões e cria a tag/release.                 |
| Isabella   | Organização e apresentação | Organiza o trabalho do grupo e cuida da apresentação final.                                             |
O projeto utiliza o Git para registrar as alterações e o GitHub para hospedar o repositório e facilitar o trabalho em equipe.

## Projeto de inspiração

* Projeto original: https://github.com/Honey-git/FloodMonitor
* Nosso fork: https://github.com/isabel684755/FloodMonitor
* O que aproveitamos: a forma de documentar os níveis de risco, explicando a regra de cada nível (Safe, Warning e Danger no FloodMonitor), e a organização do README em seções.
* Diferença: o FloodMonitor usa sensor físico e validação estatística; o nosso sistema é um protótipo educacional, sem sensores reais.
- **v1.0.0** — Primeira versão estável do sistema de monitoramento do Rio Una.

---

**Projeto educativo desenvolvido para estudar programação, versionamento e monitoramento ambiental no contexto de Palmares, Pernambuco.**
