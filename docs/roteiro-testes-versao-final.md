# Roteiro de testes da versão final

Este documento orienta a conferência do Sistema de Monitoramento do Rio Una antes da apresentação. O projeto é um protótipo acadêmico que utiliza medições simuladas ou cadastradas manualmente, e não substitui avisos oficiais.

## Testes a realizar

1. Abrir o sistema no navegador e verificar a exibição do nível atual, situação e local monitorado.
2. Clicar em **Simular medição** e conferir a atualização do nível, histórico, gráfico e aviso.
3. Digitar um valor válido em **Nível do rio (m)**, clicar em **Registrar medição** e conferir a mensagem de confirmação.
4. Tentar registrar um campo vazio ou valor negativo e verificar se o sistema impede o registro.
5. Recarregar a página após registrar uma medição e verificar se o histórico continua disponível no mesmo navegador.
6. Clicar em **Exportar histórico** e conferir se um arquivo CSV é baixado.
7. Alternar entre **Modo escuro** e **Modo claro**.
8. Verificar se a página é utilizável em uma tela menor, como a de um celular.
9. Conferir as informações do README.md, CHANGELOG.md e CONTRIBUTING.md.

## Registro da revisão

A pessoa revisora deve registrar no Pull Request o que realmente testou, quais itens funcionaram e quais precisam de correção. Se encontrar problemas, use **Request changes** ou deixe um comentário antes da integração. Se tudo estiver correto após a revisão, use **Approve**.

**Atenção:** este documento é apenas o roteiro. A execução dos testes e a aprovação precisam ser feitas pela pessoa revisora; nenhum resultado está presumido.
