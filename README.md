# NSL-KDD-Dataset




Abstract
--------

Um HIDS (Host Intrusion Detection System) é um sistema de detecção de intrusões que monitora e analisa atividades suspeitas ou maliciosas em um único host ou dispositivo. Ele é projetado para proteger o host em si, em oposição a um IDS de rede que monitora o tráfego de rede em busca de atividades suspeitas em toda a rede. O projeto consistiu na análise do DataSet NSL-KDD. O NSL-KDD possui uma ampla variedade de tráfego de rede simulado, incluindo registros normais e ataques simulados. Ele contém no total 41 atributos, dos quais 34 são numéricos e 7 são categóricos. Os ataques presentes no conjunto de dados são classificados em quatro categorias principais: DoS (Denial of Service), Probe, R2L (Remote to Local) e U2R (User to Root). O conjunto de dados também contém instâncias normais, que representam o tráfego legítimo da rede. O objetivo do projeto foi a análise desse DataSet e o treinamento de uma MLP para idenditificar possíveis eventos anômalos que pudessem representar falhas de segurança nas rotinas do servidor. Primeiramente foi abordado uma solução utilizando Decision Trees básico do SkLearn, e em seguida, a solução usando TensorFlow/Keras e Redes Neurais Artificiais para fins de comparação entre diferentes classificadores. Existem ainda outras soluções básicas usando apenas Sklearn, tais como: RandomForestClassifier, GaussianNB, KNeighborsClassifier que foram usadas também para comparação de resultados. Com o PySpark não consegui ajustar corretamente e fazer as configurações necessárias.

Data Files
----------

**KDDTrain+.ARFF** - The full NSL-KDD train set with binary labels in ARFF format

**KDDTrain+.TXT** - The full NSL-KDD train set including attack-type labels and difficulty level in CSV format

**KDDTrain+_20Percent.ARFF** - A 20% subset of the KDDTrain+.arff file

**KDDTrain+_20Percent.TXT** - A 20% subset of the KDDTrain+.txt file

**KDDTest+.ARFF** - The full NSL-KDD test set with binary labels in ARFF format

**KDDTest+.TXT** - The full NSL-KDD test set including attack-type labels and difficulty level in CSV format

**KDDTest-21.ARFF** - A subset of the KDDTest+.arff file which does not include records with difficulty level of 21 out of 21

**KDDTest-21.TXT** - A subset of the KDDTest+.txt file which does not include records with difficulty level of 21 out of 21


References
----------
[1] M. Tavallaee, E. Bagheri, W. Lu, and A. Ghorbani, “A Detailed Analysis of the KDD CUP 99 Data Set,” Submitted to Second IEEE Symposium on Computational Intelligence for Security and Defense Applications (CISDA), 2009. 

[2] J. McHugh, “Testing intrusion detection systems: a critique of the 1998 and 1999 darpa intrusion detection system evaluations as performed by lincoln laboratory,” ACM Transactions on Information and System Security, vol. 3, no. 4, pp. 262–294, 2000.
