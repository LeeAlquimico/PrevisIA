<div align="center">
  <img src="https://github.com/LeeAlquimico/PrevisIA/blob/main/EF6LxD5XoAACqUU-removebg-preview.png" alt="Descrição da Imagem" style="margin: auto;">
</div>






# PrevisIA - BUDA 3.0

## Previsão de Sequências utilizando MLP no BUDA

#### Este programa demonstra a aplicação de um Multilayer Perceptron (MLP) para a previsão de sequências.

##### Funcionalidades do BUDA:

- Carrega dados de sequências: O programa carrega dados de sequências a partir de um arquivo CSV.
- Treina um modelo MLP: Um modelo MLP é treinado utilizando os dados de sequências carregados.
- Prediz sequências: O programa prevê a próxima sequência com base em uma sequência inicial fornecida.
- Imprime sequências previstas: As sequências previstas são impressas em ordem crescente de probabilidade.

## Observações:
- Ele utiliza a biblioteca scikit-learn e é escrito em Python.
- Este programa é um protótipo e pode conter erros.
- O programa utiliza MLP é um modelo de aprendizado de máquina popular para tarefas de classificação e regressão.
- A previsão de sequências é uma tarefa bastante complexa que envolve prever a próxima sequência em uma série ordenada de números.

## Detalhes da Implementação:
### Python 3.10
##### Acesse o site oficial:  https://www.python.org/downloads/
#### Verifique a versão do Python:
```
python --version
```

#### Importações:

- numpy: Biblioteca para manipulação de arrays.
- pandas: Biblioteca para análise e manipulação de dados.
- sklearn.neural_network: Módulo da biblioteca scikit-learn para redes neurais artificiais.

### Instalando as bibliotecas pelo terminal (Windows):

```Python
pip install numpy pandas scikit-learn
```


### Aplicabilidade das Funções:

##### Função carrega_dados:

- Carrega dados de sequências a partir de um arquivo CSV e retorna as sequências e os rótulos como arrays NumPy.

##### Função treina_modelo:

- Cria um modelo MLP com três camadas ocultas e 1000 épocas de treinamento.
- Treina o modelo com os dados de treinamento.
- Retorna o modelo treinado.

##### Função previ_sequencia:

- Prevê a próxima sequência com base em uma sequência inicial definida pelo usuário.
- Utiliza o modelo treinado para calcular as probabilidades de diferentes sequências.
- Retorna os valores previstos em ordem crescente de sua probabilidade.

##### Função imprime_sequencias:

- Imprime as sequências previstas em ordem crescente.
###### Exemplo: Bloco if __name__ == '__main__'::

## Exemplo de Uso:
```Python
# Carrega os dados de treinamento de um arquivo .csv
X, y = carrega_dados('sequencias.csv')

# Treina o modelo BUDA
model = treina_modelo(X, y)

# Define a sequência para ser prevista
nova_sequencia = np.array([5, 3, 6, 1, 4, 2, 0, 0, 0, 0, 0, 0, 0, 0, 0])
nova_sequencia = nova_sequencia[:-1] # remove o último elemento

# Prevê a sequência completa
valores_previstos = previ_sequencia(model, nova_sequencia)

# Imprime as 10 sequências previstas em ordem crescente
num_sequencias = 10
imprime_sequencias(valores_previstos, num_sequencias)
```

## Explicação Final Direta: 
- Carrega os dados de treinamento.
- Treina o modelo MLP.
- Define uma nova sequência a ser prevista.
- Prevê a sequência completa.
- Imprime as 10 sequências previstas em ordem crescente.

## Recursos Adicionais:

- Documentação da biblioteca NumPy: https://numpy.org/doc/
- Documentação da biblioteca Pandas: https://pandas.pydata.org/docs/
- Documentação da biblioteca scikit-learn: https://scikit-learn.org/
  
#### Mais informações sobre MLP:
- https://en.wikipedia.org/wiki/Multilayer_perceptron
- https://scikit-learn.org/stable/modules/neural_networks_supervised.html

##
<div align="center">
      <p style="text-align: center; font-size: 0.8em;">Créditos da imagem: <a href="https://twitter.com/retrostark/status/117953383001485312">https://twitter.com/retrostark/status/117953383001485312</a></p>
</div>
