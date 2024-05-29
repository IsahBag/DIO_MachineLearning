# Machine Learning

*Alguns conceitos...*

**IA Geral**: Aquela que vemos nos filmes

**IA Restrita**: Sistemas de reconhecimento facial, sistemas de recomendação de produtos, sistemas de navegação, etc.

**Teste de Turing**: Testa a capacidade de uma máquina exibir comportamento inteligente, equivalente a um humano, ou indistinguível deste.

***Machine Learning x Inteligência Artificial:***

* Para ter uma IA, é necessário passar por um método ML. Portanto, por meio do ML obtemos (ou não) uma IA restrita.

### O que é Machine Learning?

* O objetivo do aprendizado de máquina é programar computadores para aprender um determinado comportamento ou padrão  automaticamente a partir de exemplos ou observações, utilizando DATASETS.
* Depende de uma base de conhecimento.

### Métodos de Machine Learning

* **Aprendizado por Reforço**: Rede neural recebe peso positivo caso execute um aprendizado positivo, caso negativo, recebe peso negativo
* ***Inteligência Artificial Restrita mais utilizada:*** redes neurais artificiais.
* ***Algoritmos Bioinspirados***:
  * Inspirados no comportamento de seres vivos em convivência social;
  * Conhecimento colaborativo/compartilhado;
  * Métodos heurísticos (não determinísticos);
  * Buscam a melhor solução global (solução ótima);
  * ***Genética***:
    * Utiliza as duas melhores soluções existentes, recombina essas soluções e faz uma mutação para verificar se é criada uma solução "filha" que seja melhor que as existentes.
  * ***Fuzzy (lógica nebulosa)***:
    * Trabalha com diferentes pontos de vista.
  * ***Valores determinísticos x heurísticos***:
    * *Determinísticos*: lógica booleana (ou V ou F)
    * *Heurísticos:* lógica difusa (vários valores entre V ou F)
* ***Redes Neurais Artificiais (RNA)***:

  * Inspirada nos neurônios	 e na interação entre neurônios;
  * Aprendizado por diferentes amostras.
* **Algoritmo Colônia de Formigas**:

  * Pode ser aplicado na navegação de robs, para que estes naveguem pelos melhores caminhos, utilizando os caminhos mais utilizados por outros robôs, utilizando esquemas de pontuação para cada caminho já explorado.

### Redes Neurais Artificiais (RNA)

* Conexão entre
  * neurônios;
  * conjunto de neurônios pré-definidos;
  * pesos que são gerados para que esses neurônios sejam treinados.
* Um neurônio computacional é um algoritmo modelado matematicamente com base no que é um neurônio biológico.
* Composição:
  * Neurônios de entradas;
  * Neurônios de saída;
  * Função que avalia todas as variáveis de entrada para gerar um valor de saída.
* **Modelos Artificiais:**
  * Por meio de um reconhecimento de um problema é possível gerar uma solução pré-determinadada.
* Dentro de um neurônio artificial possui um núcleo que realiza o processamento por meio de uma função de ativição, que recebe os dados, verifica a realidade dos mesmo, e caso seja um valor esperado a função de saída é ativada.
* *Estrutura*:
  * Sinais de entrada;
  * Pesos sinápticos;
  * Combinador linear;
  * Função de ativação;
  * Sinal de saída.

### Algoritmos Genéticos

* Inspirados em modelos baseados em comportamentos genéticos biológicos;
* Gera uma população de indivíduos, que vai ser avaliada por uma função *fitness*, a qual avalia os melhores indivíduos que foram gerados na população inicial;
* Indivíduos com melhores potenciais da população a ser recombinada *"pais"* irão recombinar e gerar *"filhos"* (elementos melhorados).
* *Etapas*:
  1. Gera uma população inicial de forma aleatória, dentro de uma região de interesse pré-definida, 
  2. Função *fitness* que irá avaliar os melhores indivíduos dentro da população inicial,
  3. Cria uma *população ordenada* de acordo com o valor da função *fitness*,
  4. Gera novos indivíduos a partir dos melhores definidos na *população ordenada*,
  5. Aplica a *mutação*, invertendo-se o valor binário de cada indivíduo,
  6. Utiliza-se a função *fitness* novamente para reavaliar os melhores dentre esses novos indivíduos criados.
* Objetiva gerar o melhor valor possível **ótimo global**;
* São modelos heurísticos;
* *Definição*: Um Algoritmo Genético (AG) é uma técnica de busca utilizada na ciência da computação para achar soluções aproximadas em problemas de otimização e busca.
* *Aplicações*:
  * Navegação robótica,
  * IA,
  * Geração de novos dados,
  * Jogos digitais,
  * Aplicações de ensinos e chatbot, gerando recombinação de perguntas e respostas para o usuário, deixando o sistema mais próximo de uma interação humanada.
* ***Implementando um AG***:
  * *Passo 0*: Gera população inicial de forma aleatória, dentro de uma região de busca;
  * *Passo 1*: Utiliza-se o método de seleção por roleta, selecionando os melhores indivíduos dada sua probabilidade;
  * *Passo 2*: Recombinação dos dois melhores indivíduos,utilizando valores binários, objetivando a geração de um indivíduo melhor que seus pais,
  * *Passo 3*: Seleciona um ponto do cromossomo para gerar uma mutação, invertendo o valor binário nesse ponto, evitando a convergência prematura do AG.
* ***Exemplo de funcinamento***: 
  * gerar soluções para o comportamento dos personagens em um game, evitando comportamentos repetidos entre os agentes, gerando comportamentos novos;
  * ensinar um agente em seu funcionamento desde o ponto "zero", aprendendo por tentativa e erro.

### Algoritmos de SVM (Máquinas de Vetores de Suporte)

* Utilizado quando alguma amostra dentro da população possui uma diferença muito grande comparada à sua classe, criando um hiperplano entre as amostras;
* *Algoritmo supervisionado*: 
  * relacionam uma saída com uma entrada com base em dados rotulados;
  * o usuário alimenta o algoritmo com pares de entrada e saída conhecidos;
  * processamento: entrada de dados -> interpretação dos resultados -> aplicação do algoritmo -> processamento dos dados -> saída dos dados.
* **RNA X SVM**:
  * na prática não há muita diferença;
  * o principal fator é o modo de estabelecer o hiperplano;
  * o SVM busca a otimização das margens do hiperplano;
  * o RNA busca o mínimo global para a redução do erro no treinamento.
* *Resultado esperado*: uma fronteira de decisão por meio de o hiperplano, otimizando as margens;
* *Vetores de suporte* são coordenadas de observação individual;
* Uma *SVM* é uma fronteira que melhor realiza duas classes.
* Existem casos onde não é possível separar as duas classes usando uma linha reta, pois uma das classes está no território da outra (outlier). Nesse caso o SVM irá ignorar valores discrepantes.

### DATASETs

* É a base para que se tenha um modelo de IA que foi treinado com base no modelo de machine learning com uma base de dados bem definida, que representa o problema;
