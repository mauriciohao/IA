# Detecção Automática de Pragas em Plantações de Café com CNN

## Sobre o Projeto

Este projeto implementa um sistema de classificação automática de pragas em plantações de café utilizando Redes Neurais Convolucionais (CNNs) e técnicas de Transfer Learning.

**Disciplina:** Inteligência Artificial - 7ºN CC - Noite  
**Professor:** Prof. Dr. Ivan Carlos Alcântara de Oliveira  
**Instituição:** Universidade Presbiteriana Mackenzie - Faculdade de Computação e Informática

## Integrantes

| Nome | RA | Email |
|------|----|-------|
| Eduardo Honorio Friaca | 10408959 | 10408959@mackenzista.com.br|
| Felipe Jiao | 10408852 | 10408852@mackenzista.com.br |
| Hao Yue Zheng | 10408948 | 10408948@mackenzista.com.br |
| Samuel Zheng | 10395781 | 10395781@mackenzista.com.br |

## Objetivos

- Desenvolver um classificador automático de pragas em imagens de folhas e frutos de café
- Implementar análise exploratória e preparação de dados em larga escala
- Aplicar técnicas de Transfer Learning com modelos pré-treinados
- Alcançar acurácia superior a 70% na classificação

## Estrutura do Projeto
O repositório é organizado para separar claramente notebooks, código-fonte, artefatos do N1, dados locais e pesos de modelos. Isso facilita a reprodução dos resultados, a avaliação do professor e a evolução do trabalho no N2 sem poluir o Git com arquivos grandes.

A pasta notebooks concentra os cadernos Jupyter. O N1_PragaCafe_EDA_Preparacao.ipynb executa toda a etapa do primeiro bimestre: extração/organização do dataset (VOC → ImageFolder), análise exploratória (contagens, gráficos, exemplos), definição dos transforms e criação dos splits estratificados 70/15/15. Um segundo caderno, N2_Treino_Avaliacao.ipynb, fica reservado para o desenvolvimento e a avaliação do classificador no segundo bimestre (treino com Transfer Learning, métricas e matriz de confusão).
