# Aprendizado-de-Máquina---Trabalho-01
# Classificação de Alarmes SCADA - Análise Comparativa de Embeddings

Este repositório contém a implementação do Trabalho 1 da disciplina de Tópicos Especiais em Aprendizado de Máquina. O código avalia o desempenho de três representações textuais na classificação automatizada de eventos operacionais.

## Dataset
Arquivo `chamados_scada.csv` com 150 registros sintéticos de operação de sistemas (ex: Elipse Water), divididos em três classes:
- `incidente_critico`
- `manutencao_rotina`
- `evento_informativo`

## Representações Avaliadas
1. **TF-IDF:** Representação esparsa (frequência de termos).
2. **Word2Vec:** Representação densa estática (Gensim).
3. **BERTimbau:** Representação densa contextual nos modos Feature-Based e Fine-Tuning Completo (Hugging Face).

## Requisitos e Execução
Instale as dependências executando:
```bash
pip install pandas numpy scikit-learn transformers datasets torch gensim accelerate
