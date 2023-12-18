![image](https://github.com/oumaimachabbat/TP4/assets/100364598/fe4ad304-a312-4151-8609-f6defef5bc0d)

##Pour un service de confguartion les dependances nécessaire sont :
•	Consul Discovery :
•	Spring Boot Actuator :
•	Config server : 
Pour l service (cusomer inventory order ) :
•	H2
•	JPA data 
•	Spring web 
•	Repository
•	Config client 
•	Consul 
•	Acyuator 
Pour le gateway :
•	Consul
•	Gateway
•	Actuator
##1ere etape : creation d’un dossier vide 

2- etape craetion des services 
3- Démarrer Consul ☹adreese de la machne : consul agent -server -bootstrap-expect=1 -data-dir=consul-data -ui -bind=
![image](https://github.com/oumaimachabbat/TP4/assets/100364598/2b845945-4ad3-4b53-9ab1-6674dfc2d054)

![image](https://github.com/oumaimachabbat/TP4/assets/100364598/cc82e032-56f8-41d1-8bf8-9cec24c76c04)
4- creation d’un service de configuration : @EnableConfigServer 
5- creation d’un dossier local / git pour faire la configuration :
 config-repo (les fichiers de configuration) :
•	Application .properties : les propriétés qui seront partagé partout lles microservices
6- dans le fichier . properities existant dsn l dossier ressoureces : on va déclarer le dossier ou existe la configuratyyion 
7- confiuration de service customers 
![image](https://github.com/oumaimachabbat/TP4/assets/100364598/208829a6-465e-4ced-a3cb-bf11e71fb4a2)
•	Si je fais des changement il faut faire un commit pour gardere les changements 
•	Actuatr permet de se rafrichir automatiquement avec une requête post 
![image](https://github.com/oumaimachabbat/TP4/assets/100364598/0e206a63-e3c0-4135-9ff7-49a6cdb0f3ed)
![image](https://github.com/oumaimachabbat/TP4/assets/100364598/0662a8e7-64ed-4fb8-8330-75bb88f33915)
![image](https://github.com/oumaimachabbat/TP4/assets/100364598/0bf0c4c0-9ae4-4553-8d89-232f8ba1d222)
![image](https://github.com/oumaimachabbat/TP4/assets/100364598/17b109b3-48d6-455d-b2e2-bfe8bf880480)
![image](https://github.com/oumaimachabbat/TP4/assets/100364598/93f5f0d5-81d3-4f6e-9dd1-eb17d660b7e2)
![image](https://github.com/oumaimachabbat/TP4/assets/100364598/7b69390c-741a-4661-bdbc-f3706b5b9677)
![image](https://github.com/oumaimachabbat/TP4/assets/100364598/ec25fa4e-05ea-4bd6-8e03-f14ba67d8f27)
•	Service Gateway : maintenant on va contacter les services via la gateway : 
•	Dans chaque micro Service fonctionnel o doit créer un fichier projection :









