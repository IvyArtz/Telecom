Projeto: Análise de Evasão de Clientes (Churn)

Este projeto foi desenvolvido como parte de um desafio proposto pela Alura. O objetivo é analisar uma base de dados de uma empresa de telecomunicações para identificar padrões que levam à evasão de clientes (churn) e oferecer recomendações baseadas nos dados.

Objetivo

Compreender os fatores que influenciam o churn e sugerir estratégias para reduzi-lo, contribuindo para a retenção de clientes e melhoria dos serviços prestados.

Etapas do Projeto

1. Introdução

Apresentação do problema de churn.

Importância da análise para o negócio.

2. Limpeza e Tratamento de Dados

Remoção de valores ausentes.

Conversão de colunas para tipos apropriados.

Análise exploratória inicial com info() e describe().

3. Análise Exploratória de Dados (EDA)

Gráficos de distribuição de churn:

sns.countplot(data=df, x='Churn')
plt.title('Distribuição de Churn')
plt.show()

Gráfico de churn por tipo de contrato:

sns.countplot(data=df, x='TipoContrato', hue='Churn')
plt.title('Churn por Tipo de Contrato')
plt.show()

Gráfico de churn por suporte técnico:

sns.countplot(data=df, x='SuporteTecnico', hue='Churn')
plt.title('Churn por Suporte Técnico')
plt.show()

Heatmap de correlação entre variáveis numéricas:

sns.heatmap(df.corr(numeric_only=True), annot=True, cmap='coolwarm')
plt.title('Correlação entre Variáveis Numéricas')
plt.show()

4. Conclusões e Insights

Contratos mensais estão mais associados ao churn.

Ausência de serviços adicionais é um fator de risco.

Clientes mais antigos tendem a permanecer.

5. Recomendações

Oferecer planos de fidelização para contratos mensais.

Estimular a adesão a serviços como suporte técnico.

Criar ações preventivas para clientes em risco.

Tecnologias Utilizadas

Python

Pandas

Seaborn

Matplotlib

Jupyter Notebook

Como Executar

Clone este repositório.

Certifique-se de que possui Python instalado.

Instale as dependências com pip install -r requirements.txt (opcional).

Execute o notebook aluraChallengeTelecom.ipynb em um ambiente Jupyter ou Google Colab.

Contribuição

Sugestões e melhorias são bem-vindas! Sinta-se livre para abrir issues ou pull requests.

Licença

Este projeto é livre para uso educacional e pessoal. Atribuições à autora são sempre bem-vindas.

