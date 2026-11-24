# População das Províncias de Moçambique (Censos 1997, 2007 e 2017)

Projecto em Python e SQL que analisa a evolução da população das 11 províncias de Moçambique, com dados dos três últimos recenseamentos do INE.

## Pergunta

Que províncias crescem mais depressa, e como mudou o peso de cada uma no país?
## O que o projecto faz

- Guarda os dados dos censos numa base de dados SQLite.
- Usa consultas SQL para o ranking de população, o crescimento entre censos e o peso de cada província no total.
- Calcula a taxa de crescimento anual média (2007-2017).
- Inclui um gráfico com a população e o crescimento por província.

## Como executar

```bash
python analise_populacao.py
```

Usa apenas bibliotecas incluídas no Python (`sqlite3`).

## Fonte dos dados

Instituto Nacional de Estatística de Moçambique (INE), recenseamentos gerais da população de 1997, 2007 e 2017.

## Resultados

Taxa de crescimento anual média, 2007-2017:

| Província | % ao ano |
|---|---|
| Maputo | 4,70 |
| Niassa | 3,88 |
| Tete | 3,64 |
| Cabo Delgado | 3,51 |
| Nampula | 3,24 |
| Sofala | 2,95 |
| Manica | 2,75 |
| Zambézia | 2,65 |
| Inhambane | 1,35 |
| Gaza | 1,23 |
| Maputo Cidade | -0,13 |

![Gráfico da população das províncias](grafico_populacao.png)

## Observações

- Nampula e Zambézia concentram cerca de 39% da população em 2017.
- A província de Maputo foi a que mais cresceu entre 2007 e 2017 (58,3% no total). Os dados por distrito mostram grande crescimento à volta da capital, o que sugere expansão urbana.
- Maputo Cidade foi a única a diminuir (-1,3%). Os dados não permitem concluir a causa.
- Gaza e Inhambane tiveram o crescimento mais baixo.

## Limitações dos dados

- Os valores não estão corrigidos para a população não contada. O INE estima uma omissão média de 3,7% em 2017, por isso o total oficial ajustado é superior à soma das províncias aqui usada (26,9 milhões).
- Algumas variações entre censos resultam de mudanças nas fronteiras dos distritos.

## Próximos passos

- Analisar a população ao nível dos distritos.
- Acrescentar projecções do INE para os anos seguintes.
- Gerar um relatório em Excel com as tabelas.

## Autor

Lenine João Miranda

Licenciado em Matemática (Estatística) | Análise de dados com Python e SQL | Moçambique
