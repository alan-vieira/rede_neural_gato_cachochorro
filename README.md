# 🐱 vs 🐶 Classificação de Imagens com Inception V3 (Transfer Learning)

## 📖 Visão Geral

Este projeto implementa uma solução de Visão Computacional para classificar imagens de cães e gatos. A principal estratégia utilizada foi o **Transfer Learning** (Aprendizagem por Transferência), utilizando a poderosa arquitetura **Inception V3** desenvolvida pelo Google, pré-treinada no dataset **ImageNet**.

## 🧠 Arquitetura e Metodologia

- **Modelo Base**: Inception V3 (congelado para preservar os pesos aprendidos em 1.000 categorias diferentes).

- **Customização**: Adição de uma camada de Global Average Pooling seguida de camadas densas (Fully Connected) para a classificação binária final.

- **Otimizador**: **RMSprop** (Root Mean Square Propagation), escolhido por sua eficiência em lidar com taxas de aprendizado adaptativas em redes profundas.

- **Função de Perda**: Binary Crossentropy.

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**

- **TensorFlow / Keras**: Construção e treinamento da rede neural.

- **Matplotlib**: Visualização das métricas de treinamento (Acurácia e Loss).

- **NumPy**: Manipulação de tensores e arrays.

## 🚀 Como Executar

1. Clone o repositório:

```
git clone https://github.com/alan-vieira/rede_neural_gato_cachochorro.git
```
2. Instale as dependências:

```
pip install tensorflow matplotlib numpy
```
3. Abra o Jupyter Notebook ou Google Colab e execute o arquivo:

```
rn_gato_cachorro_inception_v3.ipynb
```

## 📊 Resultados Esperados

O uso da Inception V3 permite que o modelo alcance uma alta acurácia em poucas épocas, uma vez que as camadas iniciais já são especialistas em extrair características como bordas, texturas e formas complexas das imagens.
