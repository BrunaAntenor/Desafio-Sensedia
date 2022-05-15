# O que é arquitetura monolítica ou sistema legado?
É um sistema com todas as funcionalidades, recursos  e códigos armazenados em um único local  e com o uso de apenas um único banco de dados para guardar informações. Devido a sua estrutura sua manutenção também ocorre em apenas um lugar e esse é um grande desafio desse tipo de sistema, pois se houver alguma falha em qualquer parte da funcionalidade do código, ele como um todo para de funcionar. Por ser um sistema grande e complexo, demanda mais tempo para identificar o problema e repará-lo, fato conhecido como ‘’ponto único de falha’’.

## Vantagens:
>* Simplicidade em sua arquitetura; 
>* Desenvolvimento mais rápido; 

## Desvantagens:
>* Base de códigos gigantes; 
>* Único ponto de falha; 
>* Sistema totalmente dependente de uma única linguagem de programação; 
>* Possui um único banco de dados; 

![](https://github.com/BrunaAntenor/Desafio-Sensedia/blob/main/imagens/arquitetura-monolitica.png?raw=true)

# O que é arquitetura de microsserviços?
Nesse tipo de arquitetura, cada microsservico possui sua própria regra de negócio e seu próprio banco de dados e que podem conversar através das chamadas **APIs**, por exemplo, que funcionam como um tipo de ‘’ponte’’, para se comunicar entre si. Caso um desses serviços deixe de funcionar, os outros permanecem desempenhando suas funções normalmente, o que seria uma vantagem comparado a outro tipo de arquitetura, já que apenas um serviço ficaria fora do ar.

* **API** -  *Application Programming Interface, ou, em português, interface de programação de aplicações, um conjunto de definições e protocolos para criar e integrar softwares de sistemas.* 

## Vantagens: 
>* Arquitetura individual simples; 
>* Sistema totalmente independente; 
>* Não se prende a uma única tecnologia; 
>* Elimina um único ponto de falha;
>* Facilidade e rapidez em sua atualização; 
>* Cada microsserviço possui seu próprio banco de dados; 


## Desvantagens: 
> * A arquitetura pode se tornar complexa se não for bem documentada;  
> * Maior custo; 

![](https://github.com/BrunaAntenor/Desafio-Sensedia/blob/main/imagens/arquitetura-microsservicos.png?raw=true)


# Quando devo utilizar?
Quando o software passa a ficar muito complexo é necessário uma equipe muito maior para sua manutenção, o que seria inviável, e é o que acontece muitas vezes  em um sistema monolítico. Com os microsserviços é possível quebrar esse único sistema em partes menores e independentes, onde cada um possui uma única responsabilidade, possibilitando melhorias no sistema e o uso de vários bancos de dados. Assim, ao se tratar de um sistema grande e complexo, seria adequado fragmentá-lo e distribuí-lo por diferentes equipes de suporte técnico.

# Como a arquitetura de microsserviços pode ser usada para modernizar sistemas monolíticos?
Esse tipo de arquitetura por possuir serviços menores com uma única regra de negócio específica que são mantidos, desenvolvidos, evoluídos e operados de forma independente, permite ao desenvolvedor escolher a linguagem mais adequada ao serviço que será realizado e também apresenta uma manutenção mais ágil. Contudo, ao se trabalhar em sistemas menores às vezes não vale a pena adequar a arquitetura de microsserviços, pois o custo para manter é mais elevado, já que é necessário uma maior infraestrutura e maior planejamento, o que no final das contas deixa de ser viável.

Outro ponto a ser observado é que esse tipo de arquitetura necessita de uma comunicação entre os serviços, que precisam estar disponíveis o tempo todo e também necessitam de uma maior atenção e trabalho na hora de colocar o sistema em funcionamento, já que todas as partes precisam ser colocadas no ar de forma individual.

Assim, para se trabalhar com esse tipo de arquitetura é preciso sentir a necessidade que um sistema monolítico tem de ser fragmentado, por ter chegado ao ponto de ser inviável a continuar realizando manutenção ou até mesmo acrescentando novas melhorias para ser mantido.
Por fim, para decidir qual o melhor tipo de arquitetura a ser utilizado é preciso muito planejamento e um mapeamento de todos os contextos da aplicação, onde cada microservico terá a sua responsabilidade, assim cada serviço passa ser altamente escalável, e possa ter a sua própria equipe.

# Fontes pesquisadas:

[Site Viceri](https://viceri.com.br/insights/microsservicos-x-arquitetura-monolitica-entenda-a-diferenca/
)

[Site Zappts](https://www.zappts.com/blog/arquitetura-monolitica-e-microsservicos/
)

[Site Atlassian](https://www.atlassian.com/br/microservices/microservices-architecture/microservices-vs-monolith 
)

[Site Redhat](https://www.redhat.com/pt-br/topics/api/what-are-application-programming-interfaces)

