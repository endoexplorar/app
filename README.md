# Visual-Search

Este repositório contém um notebook Google Colab que analisa os dados de um experimento de busca visual. O notebook importa dados de uma planilha do Google Sheets, realiza uma ANOVA, calcula estatísticas descritivas, realiza testes post hoc e realiza uma regressão linear para calcular o R². Os resultados da análise são então salvos em um arquivo de resumo.

## Descrição do Experimento

O experimento de busca visual mediu o tempo que os participantes levaram para encontrar um item alvo em meio a um número variável de itens distratores. O experimento teve duas variáveis independentes:

*   **Presença do alvo:** O alvo estava presente ou ausente na exibição.
*   **Número de itens:** O número de itens na exibição variou de 4 a 24.

A variável dependente foi o tempo de resposta, que foi medido em milissegundos.

## Descrição do Notebook

O notebook Google Colab neste repositório realiza as seguintes etapas:

1. **Importa os dados de uma planilha do Google Sheets.**
    *   O notebook usa a biblioteca `pandas` para importar os dados.
    *   Os dados são importados em um DataFrame do pandas.
2. **Limpa e prepara os dados.**
    *   O notebook converte os dados para o formato longo usando a função `melt` do pandas.
    *   O notebook então separa os fatores `Alvo` e `Itens` da coluna `Condição`.
3. **Realiza uma ANOVA.**
    *   O notebook usa a biblioteca `statsmodels` para realizar uma ANOVA de medidas repetidas.
    *   A ANOVA testa os efeitos principais de `Alvo` e `Itens`, bem como a interação entre `Alvo` e `Itens`.
4. **Calcula estatísticas descritivas.**
    *   O notebook calcula o tempo médio de resposta para cada combinação de `Alvo` e `Itens`.
5. **Realiza testes post hoc.**
    *   O notebook realiza testes t pareados com correção de Bonferroni para comparar o tempo médio de resposta para diferentes números de itens.
6. **Realiza uma regressão linear.**
    *   O notebook realiza uma regressão linear para calcular o R².
    *   O R² é uma medida de quão bem o modelo linear se ajusta aos dados.
7. **Salva os resultados em um arquivo de resumo.**
    *   O notebook salva os resultados da ANOVA, estatísticas descritivas, testes post hoc e regressão linear em um arquivo de texto.
    *   O arquivo de resumo também inclui uma discussão dos resultados.

## Como executar o Notebook

Para executar o notebook, você precisará do seguinte:

*   Uma Conta do Google
*   Uma conexão com a Internet
*   O notebook Google Colab

Para executar o notebook:

1. Abra o notebook no Google Colab.
2. Conecte-se a um ambiente de execução.
3. Execute as células no notebook.

## Resultados

Os resultados da análise são salvos no arquivo de resumo. O arquivo de resumo inclui o seguinte:

*   Uma tabela de estatísticas descritivas
*   Uma tabela de resultados da ANOVA
*   Uma tabela de resultados de testes post hoc
*   O valor de R² da regressão linear
*   Uma discussão dos resultados

## Conclusão

O notebook Google Colab neste repositório fornece uma análise abrangente dos dados do experimento de busca visual. Os resultados da análise sugerem que houve um efeito principal do número de itens e um efeito principal da presença do alvo no tempo de resposta. Também houve uma interação significativa entre a presença do alvo e o número de itens. Esses resultados são consistentes com a teoria da integração de características da atenção, que postula que as pessoas usam um processo serial e auto-terminante para procurar alvos em exibições visuais.

## Licença

Este projeto está licenciado sob a [Licença MIT](https://choosealicense.com/licenses/mit/).

## Contribuições

Contribuições para este projeto são bem-vindas. Por favor, envie um pull request ou abra um problema para contribuir.

## Contato

Se você tiver alguma dúvida sobre este projeto, entre em contato com [seu nome] em [seu endereço de e-mail].
