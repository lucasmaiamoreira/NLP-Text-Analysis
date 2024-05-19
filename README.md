# Análise de Notícias de Mercado de 2016

#### Este projeto realiza uma análise detalhada de notícias do mercado de 2016, utilizando diversas técnicas de processamento de linguagem natural (NLP) como tokenização, stemming, lematização, e reconhecimento de entidades (NER). O objetivo é explorar o conteúdo das notícias, identificar tópicos e criar visualizações para melhor entendimento dos dados.

#### Descrição do Projeto
O projeto é dividido em várias etapas, cada uma responsável por uma parte específica da análise. Abaixo está uma descrição de cada etapa:

1. Carregamento e Filtragem de Dados
Os dados são carregados a partir de um arquivo CSV contendo notícias. Em seguida, filtramos as notícias do ano de 2016 que pertencem à categoria "mercado".

2. Tokenização e Stemming
Usamos a biblioteca NLTK para tokenizar os textos e aplicar stemming usando o algoritmo RSLP. A função tokenize realiza esta tarefa.

3. Lematização
Utilizamos o Spacy para processar os textos e aplicar lematização. A função lemma filtra as stopwords e realiza a lematização dos tokens.

4. Reconhecimento de Entidades (NER)
Carregamos o modelo pt_core_news_lg do Spacy para identificar e extrair entidades, focando nas organizações mencionadas nos textos.

5. Vetorização dos Textos
Aplicamos a técnica de TF-IDF para converter os textos em vetores numéricos, utilizando a classe Vectorizer.

6. Extração de Tópicos com LDA
Usamos o algoritmo de Latent Dirichlet Allocation (LDA) para identificar tópicos nos textos. Os tópicos são atribuídos a cada notícia com a função get_topic.

7. Visualização dos Tópicos
Criamos visualizações das distribuições de tópicos e nuvens de palavras para cada tópico. Utilizamos a biblioteca WordCloud para gerar as nuvens de palavras.

8. Visualização das Entidades
Geramos nuvens de entidades para cada tópico, destacando as organizações mencionadas nas notícias.

Instruções para Execução

Instale as dependências:

```
pip install -r requirements.txt
```
Execute o notebook: Utilize um ambiente Jupyter Notebook para executar as células sequencialmente.

Visualize os Resultados: As visualizações dos tópicos e entidades estarão disponíveis ao final da execução do notebook.

#### Autor
Este projeto foi desenvolvido por Lucas Maia Moreira.

#### Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

#### Licença
Este projeto está licenciado sob a Licença MIT.