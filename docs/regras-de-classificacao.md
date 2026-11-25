# Regras de classificação do nível do rio

> Os valores abaixo são **simulados** e usados só para demonstração.
> Não representam medição real do Rio Una nem orientação oficial de risco
> ou de evacuação.

## Faixas de classificação

| Estado  | Critério de demonstração (nível simulado) | Significado                              |
|---------|-------------------------------------------|------------------------------------------|
| Normal  | menor que 2,5 m                           | Nível dentro da faixa considerada normal |
| Atenção | de 2,5 m até menos de 3,0 m               | Nível em faixa de atenção; acompanhar    |
| Alerta  | 3,0 m ou mais                             | Nível alto na simulação                  |

Os limites são inclusivos para o estado mais alto: exatamente 2,5 m já é
Atenção e exatamente 3,0 m já é Alerta. Esses valores são critérios
didáticos, não limites oficiais de segurança.

## Como o sistema usa essas regras

- **Ao abrir a página sem histórico salvo:** o sistema começa com 2,8 m (Atenção) e um histórico
  de 3 medições (08:00 com 2,4 m; 10:00 com 2,6 m; 12:00 com 2,8 m).
- **A cada clique em "Simular medição":** o nível simulado sobe
  0,1 m, o horário do computador é registrado e o sistema recalcula o
  estado, atualizando o card de nível, a situação, o aviso, o histórico e
  o gráfico.
- **Reinício do ciclo:** quando o nível passaria de 3,5 m, ele volta
  para 2,0 m.
- **Registro manual:** permite inserir um nível não negativo, arredondado a uma casa decimal.
- **Histórico:** mostra as 6 medições mais recentes, armazenadas localmente quando o navegador permite.
- **Exportação:** permite baixar o histórico em CSV.
- **Cores da situação:** verde para Normal, amarelo para Atenção e
  vermelho para Alerta.

## Mensagens de aviso

| Estado  | Título do aviso   | Texto do aviso                                              |
|---------|-------------------|-------------------------------------------------------------|
| Normal  | Nível normal      | O nível simulado está dentro da faixa considerada normal.   |
| Atenção | Nível em elevação | O nível registrado apresenta atenção no monitoramento.      |
| Alerta  | Nível de alerta   | O nível simulado atingiu ou ultrapassou 3,0 m.              |

O aviso depende apenas da faixa em que o nível está. O sistema não compara
a medição atual com a anterior.

## Exemplo de resultado

| Ação                                   | Nível | Estado  |
|----------------------------------------|-------|---------|
| Ao abrir sem histórico salvo                      | 2,8 m | Atenção |
| 1º clique em "Simular medição" | 2,9 m | Atenção |
| 2º clique                              | 3,0 m | Alerta  |
| Novo clique depois de chegar a 3,5 m   | 2,0 m | Normal  |

## Limitações da versão atual

- Não há sensor nem fonte real. Os dados são simulados ou inseridos manualmente.
- O histórico é local ao navegador e pode ser perdido ao limpar seus dados.
- O texto "Protótipo acadêmico" não indica medição em tempo real.

## Referência

Inspirado na forma como o projeto
[FloodMonitor](https://github.com/Honey-git/FloodMonitor) documenta seus
níveis de risco, explicando a regra de cada nível.

Documento original elaborado por Isabel (PR #3), atualizado para a versão 2.0.0.
