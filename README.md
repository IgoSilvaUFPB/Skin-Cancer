# Skin Cancer Analysis with Image Histograms
Este projeto utiliza imagens de câncer de pele para analisar estatísticas relacionadas à intensidade das áreas isoladas das lesões. Utilizamos histogramas e métricas estatísticas em lesões isoladas para obter insights que possam auxiliar no diagnóstico de câncer de pele.

## Dataset de Referência
- O dataset de imagens utilizado é fornecido pelo Kaggle: [Skin Cancer Dataset by Farjana Kabir Samanta](https://www.kaggle.com/datasets/farjanakabirsamanta/skin-cancer-dataset).

## Isolamento das Lesões
- Conversão para o Espaço HSV: A imagem é convertida para o espaço de cores HSV para segmentação de áreas de interesse.
- Criação de Máscara para Áreas Escuras: Definimos intervalos para identificar áreas de interesse que podem corresponder a lesões. Utilizamos uma máscara que isola as regiões escuras.
- Aplicação de Morfologia e Isolamento: Aplicamos operações de morfologia para refinar a máscara e isolar as lesões na imagem.

## Cálculo de Estatísticas de Intensidade
Com as lesões isoladas, calculamos as seguintes estatísticas nas áreas isoladas:
- Intensidade Média
- Percentil 50 (Mediana)
- Intervalo Interquartil (IQR)
- Assimetria (Skewness)
- Curtose (Kurtosis)
- Entropia do Histograma
