1. CARGAS ETL SEI/SIP 

Este artefato de software possui como principal objetivo automatizar 
a carga de dados no banco de dados SIP (unidades, usuários e hierarquização 
de unidades), SEI (unidades, contatos e parametrizações atreladas).

Pentaho é um software de código aberto para inteligência empresarial, desenvolvido 
em Java. A solução cobre as áreas de ETL (Extraction, Transformation and Load), 
reporting, OLAP e minerção de dados (data-mining). Desenvolvido desde 2004 pela 
Pentaho Corporation o software foi considerado uma das melhores aplicações para 
inteligência empresarial em 2008 pela InfoWorld (fonte: Wikipedia).


2. ESTRUTURA DA CARGA 

A estrutura deste ETL consiste em um job que por sua vez, possui internamente em sua estrutura 
2 transformações e 3 jobs, cada um responsável por executar ações de extração, transformação 
e carregamento de dados para o banco de dados, visando sempre manter a integridade do mesmo após 
a carga pois, durante seu desenvolvimento, uma engenharia reversa na estrutura do banco de dados 
foi realizada, afim de compreender com máxima clareza como a camada de controle da aplicação executa o carregamento dos dados.


3. OBSERVAÇÕES RELEVANTES

* A carga foi desenvolvida para trabalhar APENAS com o SGBD Microsoft SQL Server, logo 
não há garantia de que a mesma funcione com outros SGBDs;
* Caso queira fazer um 'port' da presente estrutura para outros SGBDs, ficaria feliz em ajudar;
* Sugestões são sempre bem-vindas! :-)