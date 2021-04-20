Para realização do trabalho final cada aluno deverá utilizar o dataset disponibilizado no moodle. 

Para realização do trabalho deve-se aplicar técnicas de transfer learning a diferentes arquiteturas CNNs por meio do treinamento realizado no dataset ImageNet. Para tanto, pode-se utilizar como exemplo os códigos que serão disponibilizados no moodle da disciplina os quais exemplificam tal abordagem. Os conceitos envolvidos em tal processo também estão explicitados nos slides da aula referente a redes neurais por convolução.

Para os experimentos deve-se seguir o protocolo elencado pelo dataset PapSmear disponibilizado no moodle. Caso o dataset não especifique uma política (protocolo) considere as primeiras 80% de amostras para treinamento e as 20% restantes para teste em cada classe. É importante salientar que para todos os experimentos os mesmos conjuntos de treinamento e teste devem ser mantidos para uma comparação adequada entre as técnicas.

As métricas a serem geradas para os experimentos são: 
   - acurácia, precisão, revocação, matriz de confusão, tempo de treinamento e teste

As arquiteturas CNNs a serem utilizadas são: 
- VGG16
- VGG19 
- ResNet50V2
- ResNet101V2
- InceptionV3
- Xception
- InceptionResNetV2
- MobileNetV2
- EfficientNetB1
- EfficientNetB2
- EfficientNetB3

Além de tais arquiteturas CNNs pré-treinadas, deve-se também gerar as deep features (camada flatten - consultar o exemplo denominado "Extract features with VGG16" no link https://keras.io/api/applications/#extract-features-with-vgg16) e testar as mesmas com os seguintes classificadores supervisionados:   
- KNN
- Gaussian Naive Bayes
- Decision Trees

Tais classificadores são implementados na biblioteca scikit-learn (https://scikit-learn.org/stable/supervised_learning.html#supervised-learning)


Como sugestão pode-se implementar uma aplicação que permita execução de tais experimentos via terminal, possibilitando o desenvolvimento de scripts de automatização. 

Exemplos: python trab-pdi -h ResNet -o results.txt
         
          python trab-pdi -h ResNet -c RandomForest -o results.txt


Para entrega final deve-se preparar uma apresentação de em média 30 minutos com desvio de 5 minutos. Tal apresentação deve ser estruturada da seguinte forma:

1. Introdução
2. Conceitos e Trabalhos Relacionados
3. Metodologia Proposta
4. Experimentos
4.1 Descrição da Base de Imagens
4.2 Cenários
4.3 Resultados e Discussões
5. Conclusões
Referências


A entrega do trabalho deve ser realizada via moodle. A mesma deve conter os seguintes arquivos:

   - README.txt - elucidando como deve ser realizada a execução do trabalho desenvolvido

   - script.sh - exemplo de script de execução de diferentes possibilidades

   - sources - todos os códigos fontes devidamente documentados e contendo nome e RA do desenvolvedor

   - sources slides - fontes dos slides gerados

   - PDF slides - arquivo PDF dos slides gerados


Obs: Caso sejam necessárias, para a execução do trabalho desenvolvido, bibliotecas adicionais deve-se incluir no README o detalhamento da utilização das mesmas para correta execução do trabalho (e.g. instalação, link para obtenção da mesma, etc).



https://keras.io/api/applications/
https://keras.io/api/applications/resnet/#resnet50v2-function