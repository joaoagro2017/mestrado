README

Resumo

O Brasil se destaca na pecuária graças ao uso de pastagens de Brachiaria spp., mas enfrenta desafios com plantas daninhas tóxicas que comprometem a produtividade e a saúde animal. Tecnologias como drones e Inteligência Artificial (IA), incluindo Redes Neurais Convolucionais (RNC) e Meta-aprendizagem Agnóstica (MAML), têm mostrado grande potencial para identificar e classificar plantas daninhas em imagens aéreas, com alta precisão.

Este trabalho busca avaliar o desempenho de RNCs e otimizadores em conjunto com MAML para recomendar algoritmos eficazes na classificação de plantas daninhas e pastagens a partir de imagens de drones. O estudo foi realizado nos municípios de São Miguel dos Campos e Tanque D’Arca, no estado de Alagoas, Nordeste do Brasil, utilizando imagens de drone do tipo ortomosaico.

Foram aplicadas técnicas como aumento de dados, oversampling, redes neurais convolucionais (RNCs) com MAML, e validação cruzada K-Fold, resultando em melhorias na precisão, no equilíbrio das classes e na generalização do modelo. Os resultados mostram que o PSO é o otimizador mais eficaz, com a melhor acurácia (57,70%) e menor tempo de processamento (101,15s). A abordagem baseada em deep learning confirma seu potencial para identificar plantas daninhas tóxicas, promovendo eficiência no manejo agrícola.

Passo a Passo de Instalação e Execução

1. Clonar o Repositório

Abra o terminal e execute:

git clone https://github.com/joaoagro2017/mestrado.git
cd <NOME_DO_DIRETORIO>

2. Criar um Ambiente Virtual (opcional, mas recomendado)

python3 -m venv venv
source venv/bin/activate # Para Linux/Mac
venv\Scripts\activate.bat # Para Windows

3. Instalar Dependências

Para garantir que todas as bibliotecas necessárias estejam instaladas:

pip install -r requirements.txt

4. Organizar o Dataset

Certifique-se de que as imagens estejam na pasta dados. e esteja separa como uma pasta para cada respectiva classe.
exemplo.

/dados/classe 1/
/dados/classe 2/
/dados/classe 3/

5. Executar os Scripts

a) pré processamento

Execute o script de pré processamento:

daninhas_extract.ipynb

b) Treinamento e avaliação (MLP)

mlp_otimizadores.ipynb

c) Visualização dos Resultados

os resultados são visualizados e exportados para um zip com todos os resultados do treinamento e avaliaçãos dos folds


Requisitos do Sistema

Python 3.8 ou superior

TensorFlow 2.9.2

PyTorch (opcional para comparativos)

RTX A1000 GPU (recomendado para alta performance)

Pacotes listados no requirements.txt

Referências

Documentação oficial do TensorFlow: https://www.tensorflow.org/

Pesquisa sobre Meta-aprendizagem: MAML

Python: https://www.python.org/