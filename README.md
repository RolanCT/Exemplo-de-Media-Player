# Exemplo-de-Media-Player
Media Player: com um Butão  Start para parar o toque e outro com Butão  stop para parar a execução





Tema: Services;

o que são  Services?
são  processo logos execuntados no background  e executados de um outro componentes.


***Utilização****: por um Intent;
caso o servico desejado seja privado , podemos cinfigurar no android manifest.


***Tipos de servicos****:
- started servicos[nao retorna resultado e interacao com o services]
 a avtivity vai ficar a espera de um processo terminar

**sao executados por uma actividity ou broadcast receivers
** usando uma Intent para iniciar um service atraves do metodo startServices();
**o terminar a opercao pode ser terminado pelo método stopService();


-{Intent services};
Os servicos por natureza são executados pela Thread pelos servicos que o invocam, apos o termino dos trabalhos e espera  que todos serviços também sao terminados.

-{Bound Services}-->[ ele permite interação com o services] vicula e termina

***Tipos de bound services****
: *bindService() : O componte é que vai iniciar e vicular o service 

 * unbindServices() : vai retornar um valor 

=e pode ser considerado assicrono=
------------------------


-=-=- ***Ciclo de vida de um Serviço****

****NB: estude os ciclos para melhor compreensão****


=====Metodo da propria classe que executam o "Service"====

-onStartcommand();
-onBind;
-onCreate();
-ondestroy;
-onhandleWork();




=== Opções  de restart do serviço:

- Start_not_Sticky;
- START_STICK;
- START_REDELIVER_INTENT;

-------------------------------------
Para que serve o metodo getContext ?
