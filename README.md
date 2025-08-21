# Winicius-
📌 Resumo do Código

O código implementa um pipeline de Machine Learning simples para simular a aprovação de crédito de clientes e, em seguida, utiliza a biblioteca LIME para explicar as decisões do modelo.

🔹 Etapas principais

Criação do Dataset

Conjunto fictício de 20 clientes com informações como:

Nome, Idade, Salário, Valor solicitado, Tempo de emprego, Histórico de crédito etc.

Variável alvo: Aprovado (Sim/Não).

Pré-processamento

Remoção da coluna Nome (não relevante para o modelo).

Transformação de variáveis categóricas em numéricas usando LabelEncoder (Empregado, Historico_Credito, Aprovado).

Separação em features (X) e target (y).

Divisão dos dados em treino e teste.

Treinamento do Modelo

Uso do Random Forest Classifier (100 árvores).

O modelo aprende padrões que indicam se o cliente terá crédito aprovado.

Explicabilidade com LIME

Criação de um LimeTabularExplainer com os dados de treino.

Seleção de uma amostra do conjunto de teste para explicação.

O LIME identifica os atributos que mais influenciaram a predição (positiva ou negativa).

As explicações são mostradas:

Diretamente no notebook (show_in_notebook), com visualização interativa.

Em formato textual (exp.as_list()), listando variáveis e pesos.

Exportadas para HTML (explicacao_lime.html) para análise fora do ambiente Python.

🎯 Para que serve

Predição: prever automaticamente se um cliente deve ter o crédito aprovado.

Explicabilidade: entender os motivos de cada decisão do modelo, garantindo transparência (fundamental em aplicações financeiras).

Análise individual: permite justificar por que um cliente foi aprovado ou negado com base em suas características.

👉 Em resumo: seu código não só treina um modelo preditivo, como também mostra o “porquê” por trás das decisões, usando o LIME como ferramenta de interpretabilidade.

Quer que eu transforme esse resumo em uma seção “📖 Como funciona o código” para incluir direto no README.md também?
