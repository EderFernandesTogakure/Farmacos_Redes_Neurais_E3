# Avaliação do polimorfismo de fármacos utilizados para produção de medicamentos através do algoritmo de machine learning.
# Polymorphism evaluation of drugs used for drug production through machine learning algorithm.
## Apresentação
  O presente projeto foi originado no contexto das atividades da disciplina de pós-graduação [Ciência e Visualização de Dados em Saúde](https://github.com/datasci4health/home), oferecida no primeiro semestre de 2021, na Unicamp.
Nome	                     |   RA	  |Especialização
---------------------------|--------|---------------
Eder Carlos Fernandes	     | 208418	|Computação
Gabriel Santos Martins Dias| 172441	|Computação
Wellen Góbi Botacin         | 224798 |Saúde
Wellington Cesar Alves     | 261819 |Saúde


## Descrição Resumida do projeto 

   Um determinado fármaco, no estado sólido, pode se apresentar em diferentes formas. Estas formas incluem polimorfos (capacidade de uma substância se apresentar em duas ou mais formas cristalinas) e amorfos (formas sólidas que não têm nenhuma ordem molecular).
   
  O fenômeno do polimorfismo apresenta um desafio na indústria farmacêutica que pretende desenvolver medicamentos de qualidade, pois o desconhecimento das diferentes formas cristalinas e a influência destas no preparo de um medicamento poderá acarretar em grandes prejuízos para a saúde do paciente. Com isso, a pesquisa na área de polimorfismo é extremamente necessária e atual, sendo um assunto que não deve ser encarado somente como um problema, mas como um processo, que deve ser estudado e monitorado, desde a síntese da substância ativa até o armazenamento, resultando em maior qualidade aos medicamentos.
  
  A capacidade de uma molécula cristalizar em duas ou mais formas é definida como polimorfismo.
  
  Polimorfos diferentes de um mesmo composto geralmente apresentam diferenças significativas de solubilidade, processabilidade e estabilidade física e química. Estas diferenças físico-químicas modificam o comportamento da molécula quando em um meio biológico, inclusive podendo alterar sua biodisponibilidade.
  
  Embora uma molécula orgânica de um sólido possa existir sob duas ou mais formas cristalinas, apenas uma destas formas é termodinamicamente estável a uma determinada pressão e temperatura, com níveis energéticos potencialmente mais baixos, devido à redução do seu volume molecular em relação aos amorfos ou outro estado desordenado. Em geral, a forma mais estável (menor energia livre) de uma substância polimórfica exibe um ponto de fusão mais alto e menor solubilidade com o máximo de estabilidade química, ou seja, mantém sua integridade química dentro de limites especificados e as mesmas propriedades e características durante o período de armazenamento e uso (RAW et al., 2004; VISHWESHWAR et al., 2006).
  
  O polimorfismo pode também resultar em alterações na estabilidade química, principalmente para compostos com predisposição à degradação no estado sólido (ARAÚJO, 2009). Porém, dentre as consequências do polimorfismo, a mais crítica é a diferença na biodisponibilidade dos diferentes polimorfos de um fármaco, uma vez que, a velocidade de absorção de um fármaco depende da sua velocidade de dissolução, podendo torná-lo menos ativo, inativo ou tóxico de acordo com o tipo de polimorfo empregado (FERREIRA, 2011; CUFFINI et al., 2011).
  
# Vídeos do Projeto

## Vídeo da Proposta

[Video de apresentação de Ciência de Dados em Saúde - Proposta](https://youtu.be/6PfZkR7TSeM).


# Slides do Projeto

## Slide da Proposta

[Slide da proposta do projeto](https://github.com/EderFernandesTogakure/Farmacos_Redes_Neurais_E3/blob/main/assets/Proposta.pptx).

# Introdução e Referenciais de Teóricos

## Contextualização do projeto

Um determinado fármaco, no estado sólido, pode apresentar-se em diferentes formas. Estas formas incluem polimorfos (capacidade de uma substância se apresentar em duas ou mais formas cristalinas) e amorfos (formas sólidas que não têm nenhuma ordem molecular).

Embora uma molécula orgânica de um sólido possa existir sob duas ou mais formas cristalinas, apenas uma destas formas é termodinamicamente estável a uma determinada pressão e temperatura, com níveis energéticos potencialmente mais baixos, devido à redução do seu volume molecular em relação aos amorfos ou outro estado desordenado. Em geral, a forma mais estável (menor energia livre) de uma substância polimórfica exibe um ponto de fusão mais alto e menor solubilidade com o máximo de estabilidade química, ou seja, mantém sua integridade química dentro de limites especificados e as mesmas propriedades e características durante o período de armazenamento e uso (RAW et al., 2004; VISHWESHWAR et al., 2006).

O fenômeno do polimorfismo apresenta um desafio na indústria farmacêutica que pretende desenvolver medicamentos de qualidade, pois o desconhecimento das diferentes formas cristalinas e a influência destas no preparo de um medicamento poderá acarretar em grandes prejuízos para a saúde do paciente. Com isso, a pesquisa na área de polimorfismo é extremamente necessária e atual, sendo um assunto que não deve ser encarado somente como um problema, mas como um processo que deve ser estudado e monitorado, desde a síntese da substância ativa até o armazenamento, resultando em maior qualidade aos medicamentos.

A capacidade de uma molécula cristalizar em duas ou mais formas é definida como polimorfismo. Polimorfos diferentes de um mesmo composto geralmente apresentam diferenças significativas de solubilidade, processabilidade e estabilidade física e química. Estas diferenças físico-químicas modificam o comportamento da molécula quando em um meio biológico, inclusive podendo alterar sua biodisponibilidade.

O polimorfismo pode também resultar em alterações na estabilidade química, principalmente para compostos com predisposição à degradação no estado sólido (ARAÚJO, 2009). Porém, dentre as consequências do polimorfismo, a mais crítica é a diferença na biodisponibilidade dos diferentes polimorfos de um fármaco, uma vez que, a velocidade de absorção de um fármaco depende da sua velocidade de dissolução, podendo torná-lo menos ativo, inativo ou tóxico de acordo com o tipo de polimorfo empregado (FERREIRA, 2011; CUFFINI et al., 2011).

Pretende-se utilizar o machine learning para esta tarefa. Proporcionando um “aprendizado” à máquina para que ela facilite este processo de reconhecimento, aproximando cada vez mais tecnologia e saúde.

## Caracterização do problema

Polimorfismo é a capacidade de um determinado fármaco no estado sólido se apresentar em duas ou mais formas cristalinas e amorfos (formas sólidas que não têm nenhuma ordem molecular). O sólido cristalino é formado por átomos, moléculas ou íons, arranjados de uma forma periódica em três dimensões, onde as posições ocupadas seguem uma ordenação que se repete, segundo uma ordem definida ao longo de toda a partícula. No estado sólido, os átomos de uma molécula podem existir em um dos sete arranjos cristalinos fundamentais: triclínico, monoclínico, ortorrômbico, romboédrico, tetragonal, hexagonal ou cúbico. 

Em outras palavras, a forma morfológica do fármaco tem a capacidade de influenciar a solubilidade do ativo no trato gastrointestinal, consequentemente alterando características de absorção que por sua vez define se haverá efeito terapêutico desejado.

O machine learning, termo que possui diversas definições, pode ser chamado aprendizado de máquina, com um sistema que pode modificar o seu comportamento com base em sua experiência, com mínima intervenção humana. Pode ser utilizado em diversas áreas, como por exemplo em bancos de dados autônomos ou combate a fraudes em sistemas de pagamento (ALMEIDA, 2021).

Dessa maneira, o intuito do trabalho conduzido é avaliar a eficiência do algoritmo machine learning, desenvolvido na identificação e quantificação de formas, unindo computação e saúde no propósito de melhorar a fabricação de medicamentos e, consequentemente, seus resultados na população. 

## Motivação

A motivação deste trabalho é desenvolver um algoritmo machine learning, que agilize esse processo de identificação do polimorfismo dos fármacos, facilitando seu processo de identificação. 

## Relevância

O fenômeno do polimorfismo representa um desafio na indústria farmacêutica que pretende desenvolver medicamentos de qualidade, pois o desconhecimento das diferentes formas cristalinas e a influência destas no preparo de um medicamento poderá acarretar grandes prejuízos para a saúde do paciente, além de prejuízos ao fabricante. 

O ponto de partida para a fabricação de fármacos é a pré-formulação, sendo a primeira fase do desenvolvimento de formas farmacêuticas voltadas para a substância farmacologicamente ativa.
Nesta fase ocorre a análise do fármaco em suas características físico-químicas como solubilidade, presença ou não de formas polifórmicas e seu comportamento frente à excipientes farmacêuticos ou outras substâncias farmacologicamente ativas.

Na indústria farmacêutica o polimorfismo é considerado um parâmetro fundamental na fabricação de medicamentos sólidos, pois a criação de um fármaco sob uma ou outra forma cristalina implica nas propriedades físico-químicas desta substância, que irão afetar diretamente a solubilidade, e consequentemente a biodisponibilidade ou cinética. 

A grande maioria dos medicamentos comercializados pelas indústrias farmacêuticas encontra-se em formas farmacêuticas sólidas de uso oral que apesar de serem de fácil administração ao paciente, necessitam que o fármaco seja biodisponibilizado em tempo adequado no organismo. Este trabalho busca, com auxílio de um algoritmo, facilitar esse processo e produzir medicamentos com maior qualidade. 

## Trabalhos relacionados

Por ser uma temática nova, ainda não existem publicações com o mesmo formato deste trabalho. Têm-se publicações semelhantes , sendo exemplos:

YOLO: Real-Time Object Detection . pjreddie, 2018. Disponivel em: < https://pjreddie.com/darknet/yolo/>. Acesso em: 26 Abr. 2021.

YOLO v3 theory explained. Pylessons, 2019. Disponível em: <https://pylessons.com/YOLOv3-introduction/>. Acesso em: 26 abr. 2021.

SHAKAMARI, A.; MENHAJ, M. B.; HORMAT, A. M.; TARRAH, H. A fast and yet efficient YOLOv3 for blood cell detection. Biomedical Signal Processing and Control, V. 66, Abril 2021.

RAUJO, G. L. B. Caracterização no estado sólido dos polimorfos de tibolona. Tese (Doutorado em Farmácia) - Faculdade de Ciências Farmacêuticas, Universidade de São Paulo, São Paulo, 2009.

CUFFINI, S. L.; PITALUGA, J. R. A; TOMBARI, D. Polimorfismo em fármacos. In: STORPIRTIS, S.; GONÇALVES, J. E.; CHIANN, C.; GAI, M. N.; editors. Biofarmacotécnica. Rio de Janeiro: Guanabara Koogan, 2011, p.21-31.

RAW, A. S; FURNESS, M. S.; GILL, D. S.; ADAMS, R. C.; HOLCOMBE JR, F. O.; YU, L. X. Regulatory considerations of pharmaceutical solid polymorphism in Abbreviated New Drug Applications (ANDAs). Advanced Drug Deliveries Amsterdam, v. 56, n.3, p. 397-414, fev. 2004.

VISHWESHWAR, P.; MCMAHON, J. A.; BIS, J. A.; ZAWOROTKO, M. J. Pharmaceutical co-crystals. Journal of Pharmaceutical Sciences, v.95, n.3, p.499516, mar. 2006.

## Pergunta de pesquisa

O algoritmo machine learning desenvolvido é eficaz na identificação de polimorfos de fármacos para auxiliar a industria farmaceutica na produção de medicamentos de melhor solubilidade?

## Objetivos do Projeto

O projeto possui como objetivo principal a criação de um algoritmo machine learning que auxilie na identificação do polimorfismo de fármacos. Busca-se também:

* Identificar se o algoritmo machine learning é eficaz nessa identificação;
* Verificar sua capacidade de identificação;
* Avaliar sua disponibilidade de utilização.

## Metodologia 
  A carbamazepina é um fármaco que apresenta baixa solubilidade, estreita janela terapêutica e exibe polimorfismo. A presença de diferentes polimorfos da carbamazepina em medicamentos está relacionada com propriedades de solubilidade de dissolução limitadas, onde apenas a forma polimórfica III deve estar presente em produtos comerciais. 
  
  Foi disponibilizada amostra de insumo farmacêutico ativo carbamazepina em sua forma polimórfica comercial III, analisada e verificada sua identidade em microscópio óptico.
Parte da amostra do insumo foi submetido à temperatura de 170°C em equipamento de Analise térmica DSC (Calorimetria exploratória diferencial) até conversão de seu estado cristalino em forma polimórfica I.

  Foram analisadas e verificadas quanto a sua identidade e confirmada presença de forma polimórfica III.
Posteriormente foram geradas as imagens utilizadas para treinamento do algoritimo a partir das duas formas polimórficas, separadamente e com misturas realizadas entre elas, em microscópio ótico acoplado a software de captação de imagens.

  Obtenção da Base de Dados: Foi utilizado um Microscópio Óptico para se obter dezenas de imagens. Em seguida, sobre essas imagens, foi utilizado o processo de Data Augmentation (Aumento de dados de imagem) para gerar novas imagens de treinamento a fim de aumentar a generalidade do modelo e reduzir um possível overfitting (modelo treinado apenas para imagens utilizadas no estudo). 
  
  Foram produzidas imagens a partir de pequenas transformações nos arquivos obtidos no Microscópio Óptico e foi possível compor um conjunto de base de treinamento com centenas de imagens. 
Abaixo, segue imagem ilustrando o processo.

![relatório](https://user-images.githubusercontent.com/25067632/120075355-4ec35f00-c077-11eb-9fa7-cd96279ef307.jpg)

  

## Ferramentas

  As ferramentas que serão utilizadas neste projeto são:
  
  * Jupyter Notebook: Aplicação web utilizada como IDE. O Jupyter Notebook fornece um ambiente de ciência de dados interativo e fácil de usar em muitas linguagens de programação que não funciona apenas como um IDE, mas como uma  ferramenta didática;
  * Google Colab: Ambiente de programação que fornece um poderoso recurso de computação científica  para executar códigos de Machine Learning a partir de uma GPU presente no servidor;
  * Pythorch: Biblioteca de programação de código aberto usada para desenvolvimento de softwares de Machine Learning e Deep Learning;
  * YOLO: Biblioteca de código aberto de visão computacional utilizada para detecção e classificação de objetos em tempo real;
  * Darknet: Arquitetura de rede neural profunda utilizada no YOLO;
  * OpenCV:Biblioteca de programação de código aberto amplamente empregada no desenvolvimento de aplicativos na área de visão computacional;
  * Microscópio Óptico: Utilizado para fazer a captura de um conjunto de 20 imagens de 2 compostos distintos. 

## Detalhamento e evolução do projeto

O projeto irá adotar tecnologia baseada em redes neurais convolucionais, ou seja, para um melhor entendimento, inteligência artificial em conjunto com processamento de imagem
Veja a figura abaixo uma figura demonstrando os passos para elaboração do projeto.

![imagem_projeto2](https://user-images.githubusercontent.com/25067632/113519557-6d1f4980-9563-11eb-8c51-af6f37edc15c.jpg)

Será detalhado todos os processos da imagem acima:

* Primeiro tópico obtendo datasets. Os datasets são as imagens que serão inseridas no sistema para o treinamento da detecção dos polimorfos, quanto mais imagens forem obtidas para o treinamento e teste, maior será a precisão da detecção;
* O pré-processamento e aumento das imagens. Nesta etapa, são extraídas as imagens originais, ou seja, os datasets das imagens são inseridos no sistema e faz as cópias delas com pequenas alterações nos arquivos para aumentar a precisão das detecções;
* Classificação das imagens. Esta etapa é muito importante para um bom treinamento da rede neural convolucional, pois somente inserir as imagens no sistema não é o suficiente. Deve-se classificar os compostos dentro da imagem a serem treinados, ou seja, demonstrar cada polimorfo, demarcando-os com uma ferramenta específica de classificação;
* Processo de execução dos treinos e testes de validação de dados. Nesta etapa do processo, é realizado o treinamento da rede neural convolucional, ou seja, está sendo ensinado como detectar os compostos descritos na imagem;
* Execução dos dados treinados e validados em produção. Esta é a etapa final, na qual a rede neural foi treinada e agora fará a detecção dos polimorfos da maneira que foi programada. 

## Bases de Dados e Evolução
  As bases de dados utilizadas serão imagens de processos de identificação de componentes fármacos feitas em microscópios óticos de forma manual. 
## Bases Estudadas e Adotadas
As bases de dados estudadas foram imagens de analise reais de polimorfos farmacos, na qual foram feitas pelo farmaceuto da equipe.

Com estas imagens adquiridas foram feitos os devidos aumentos de dados destas imagens, para serem  utilizadas para treinamento, teste e validação dos componentes farmaceuticos.

Com o treinamento, testes e validação destes dados foi descoberto que é possivel fazer a deteção dos polimorfos farmacos, logo agilizando o processo de identificação do mesmo. 

Base de Dados              |  Endereço na Web  |Especialização
---------------------------|-------------------|---------------
Imagens Carbazepina e planilha analise         | https://github.com/EderFernandesTogakure/Farmacos_Redes_Neurais_E3/tree/main/data	           |Imagens tirados diretos do microscopio forma 1 e 3,foi separado as imagens de treino e teste, utilizando redes neurais convolucionais para detecção dos fármacos.

## Análises realizadas 

O projeto foi motivado em razão da dificuldade de identificação de formas polimorficas em diversos fármacos.

O processo de identificação dos polimorfos farmacêuticos é feito de forma visual por um especialista, na qual foi pensado em automatizar este processo para ter um melhor controle de qualidade sobre estes fármacos.

Foram feitas imagens de análises reais do fármaco Carbamazepina com dois tipos de polimorfos, os quais foram denotados como forma 1 e forma 3. Com estas imagens elaboradas foram feitas os seus aumentos de dados com pequenas distorções nas imagens a fim de obter uma boa performance no treinamento.

Foram utilizado o modelo do YOLOv3 para treinamento, teste e validação destas imagens, veja logo abaixo um trecho do notebook para fazer o treinamento das imagens.

![cod1](https://user-images.githubusercontent.com/25067632/123013086-e0ce3700-d399-11eb-9d0d-9c93353c01bd.jpg)

Depois de feito o treinamento e teste do modelo, foi elaborado a validação no trecho do notebook logo abaixo

![cod2](https://user-images.githubusercontent.com/25067632/123013428-95685880-d39a-11eb-90ae-5174e41a7a94.jpg)

Veja o resultado da predição na imagem abaixo

![download](https://user-images.githubusercontent.com/25067632/123012748-37874100-d399-11eb-9856-b883afd3c212.png)

Após o modelo ter sido treinado, foram feitas as validações das imagens para testar o modelo. De forma visual, foram levantados os seguintes resultados sobre a saída do modelo:
* O software não classificou nenhuma forma polimórfica da forma errada, isto é, não confundiu a forma 1 com a forma 3 nem a forma 3 com a forma 1;
* Os erros do software ocorreram quando ele não foi capaz de fazer a delimitação de uma caixa delimitadora em uma forma polimórfica;
* De todas as formas presentes nas imagens, o Software identificou 74,8% delas e não foi capaz de identificar 25,2% delas. 

![WhatsApp Image 2021-06-22 at 21 54 24](https://user-images.githubusercontent.com/25067632/123018387-d7969780-d3a4-11eb-9d20-a105e4657d6b.jpeg)

![grafico](https://user-images.githubusercontent.com/25067632/123017790-aec1d280-d3a3-11eb-88cc-da1d07519d20.jpeg)


## Resultados/discussão

  Na determinação do polimorfismo da Carbamazepina utilizando a ferramenta proposta, a exatidão dos resultados encontrados em comparação a avaliação de especialista, estabeleceu-se em 75% de acerto.
  
  Foi observada pequena variação nos resultados, sendo mais eficiente para avaliação e identificação da forma polimórfica III.
  
  Compreendemos e admitimos que a ferramenta proposta se mostra viável, de acordo com os resultados encontrados. E entendemos também, que há possibilidade de melhora de eficiência de identificação, principalmente com a ampliação do numero de imagens para treinamento do algoritmo proposto.

## Conclusão

Na determinação do polimorfismo da Carbamazepina utilizando a ferramenta proposta, a exatidão dos resultados encontrados em comparação a avaliação de especialista, estabeleceu-se em 75% de acerto.

Foi observada pequena variação nos resultados, sendo mais eficiente para avaliação e identificação da forma polimórfica III.

Compreendemos e admitimos que a ferramenta proposta de mostra viável, de acordo com os resultados encontrados. E entendemos também, que há possibilidade de melhora de eficiência de identificação, principalmente com a ampliação do numero de imagens para treinamento do algoritmo proposto.

## Trabalhos futuros

* Elaborar artigos cientificos;
* Aprimorar a ferramenta;
* Patentear a ferramenta.

## Referências:

ARAUJO, G. L. B. Caracterização no estado sólido dos polimorfos de tibolona. Tese (Doutorado em Farmácia) - Faculdade de Ciências Farmacêuticas, Universidade de São Paulo, São Paulo, 2009. 

CUFFINI, S. L.; PITALUGA, J. R. A; TOMBARI, D. Polimorfismo em fármacos. In: STORPIRTIS, S.; GONÇALVES, J. E.; CHIANN, C.; GAI, M. N.; editors. Biofarmacotécnica. Rio de Janeiro: Guanabara Koogan, 2011, p.21-31.

Documentação do tensorflow. Tensorflow, 2021. Disponível em: <https://www.tensorflow.org/api_docs/python/tf?hl=pt-br>. Acesso em: 26 abr. 2021.

FERREIRA, A. O. Guia Prático da Farmácia Magistral. 4. ed. São Paulo: Pharmabooks, 2011. 736 p.

RAW, A. S; FURNESS, M. S.; GILL, D. S.; ADAMS, R. C.; HOLCOMBE JR, F. O.; YU, L. X. Regulatory considerations of pharmaceutical solid polymorphism in Abbreviated New Drug Applications (ANDAs). Advanced Drug Deliveries Amsterdam, v. 56, n.3, p. 397-414, fev. 2004.

VISHWESHWAR, P.; MCMAHON, J. A.; BIS, J. A.; ZAWOROTKO, M. J. Pharmaceutical co-crystals. Journal of Pharmaceutical Sciences, v.95, n.3, p.499516, mar. 2006.

YOLO v3 theory explained. Pylessons, 2019. Disponível em: <https://pylessons.com/YOLOv3-introduction/>. Acesso em: 26 abr. 2021.

YOLO: Real-Time Object Detection . pjreddie, 2018. Disponivel em: < https://pjreddie.com/darknet/yolo/>. Acesso em: 26 Abr. 2021

SHAKAMARI, A.; MENHAJ, M. B.; HORMAT, A. M.; TARRAH, H. A fast and yet efficient YOLOv3 for blood cell detection. Biomedical Signal Processing and Control, V. 66, Abril 2021.














