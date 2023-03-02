# Análise de Regressão Simples e Múltipla

Teste dos parâmetros dos modelos: Alfa e Beta
  - Teste F: teste de hipótese para os parâmetros Beta
           -> H0 = todos os Betas = 0 (B1 = B2 = B3 = 0)
           -> H1 = pelo menos um Beta é diferente de zero
           -> Nível de confiança de 95%
  - Teste t-Student: teste de significância para todos os parâmetros do modelo (Alfa e Beta)
          -> H0 = Beta = 0
          -> H1 = Beta estatisticamente diferente de zero
          -> Nível de confiança de 95%
          
R² e R² Ajusted: coeficiente de explicação do modelo

One-hot enconding ou Dummização: alteração das variáveis categóricas em valores binários (0-1)

Procedimento Step-Wise: processa o modelo com reduçao da multicolinearidade

Teste de Shapiro-Wilk ou Shapiro-Francia: teste de aderência dos termos de erro a normalidade
        -> H0 = não há diferença da distribuição dos termos de erro e a curva normal
        -> H1 = há diferença estatistica da distribuição dos termos de erro a curva normal
        Aceitamos o modelo que rejeita H1 ou aceita H0
        
Transformação Box-Cox: transforma a variável dependente em um valor que maximiza a aderência dos termos de erro a normalidade
        -> valor de lambda -inf +inf

Teste Variance Inflation Factor e Tolerance: teste de multicolinearidade das variáveis independentes
        -> Tolerance mais perto de 1

Teste Breusch-Pagan: teste de heterocedasticidade dos termos de erro
        -> Quando os termos de erros são significantes, pode haver omissão de variáveis explicativas relevantes ao modelo, mas que no momento estão sendo omitidas.
        -> u = está fazendo o papel de uma variável independente omitida
