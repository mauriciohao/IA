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
.
├── README.md
├── .gitignore
├── notebooks/
│   ├── N1_PragaCafe_EDA_Preparacao.ipynb     # EDA + preparação (Parte 2 / N1)
│   └── N2_Treino_Avaliacao.ipynb             # (placeholder) treino + métricas (N2)
├── src/
│   ├── data_prep/
│   │   ├── voc_to_imagefolder.py             # VOC (JPEGImages+Annotations) → ImageFolder (classes)
│   │   └── gen_crops_from_voc.py             # (opcional) crops por bounding boxes → ImageFolder
│   ├── training/
│   │   └── train_classifier.py               # (N2) treino com ResNet/MobileNet e avaliação
│   └── utils/
│       ├── transforms.py                     # transforms de imagem (resize/normalize/augment)
│       └── metrics.py                        # precisão/recall/F1, matriz de confusão
├── reports_n1/
│   ├── class_counts.csv                      # contagem por classe (EDA)
│   ├── dataset_card.md                       # resumo das decisões de preparação
│   ├── figures/
│   │   ├── distribuicao_top_classes.png      # gráfico de distribuição (Top-N)
│   │   └── exemplo_<classe>.png              # amostras visuais salvas
│   └── splits/
│       ├── train.csv                         # listas estratificadas (path, class_idx, class_name)
│       ├── val.csv
│       └── test.csv
├── data/                                     # (IGNORADO no Git)
│   ├── data_ip102_raw/                       # ZIP extraído (VOC): JPEGImages/ e Annotations/
│   └── data_ip102/
│       ├── images/                           # ImageFolder final (classes) — usado no N1
│       └── images_crops/                     # (opcional) ImageFolder com crops por objeto
└── models/                                   # (IGNORADO no Git) pesos treinados (.pth) — N2

