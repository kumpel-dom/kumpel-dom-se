# Breve explicação dos campos e valores aceitos

Haverá dois tipos de documentos _json_, o primeiro será utilizado para iniciar os aplicativos que fazem parte do sistema. Quando o sistema for inicialmente configurado, será gerado um documento json assim como dados e configurações de persistência, nesse documento havera todas as infoemações necessárias para o funcionamento do sistemas em todas as plataformas abrangentes. Já o segundo documento será para aplicar alguma ação ao sistema. Como por exemplo apagar uma luz ou acionar o alarme.

## Campos

 * **nodeid**: Será usado pelo sistema para identificar cada nó e suas ações. Valor aceito:
      - números inteiro


 * **nodename**: Para facilitar a utilização do sistema, um nome de fácil assimilação será armazenado e mostrado para o usuário. Valor aceito:
     - Strings


 * **area**: Um nó será capaz de controlar mais de uma area da residência, para isso cada area terá que ter sua própria identificação e cinjunto de ações;


 * **areaid**: Da mesma forma que será necessário um identificador para cada nó, o mesmo é verdade para cada area. Valor aceito:
    - números inteiro


 * **areaname**: Ainda para facilitar a utilização, deicando o sistema mais intuitivo, o usuário nomeará cada area. Por exemplo, o _id_ 1 terá o nome de sala. Dessa forma o usuário não precisará memorizar o que é cada area e o que elas fazem. Valor aceito:
     - Strings


 * **actions**: Cada area será responsável por executar suas ações e reportar ao sevidor as ações executadas;


 * **actionid**: Identificação de cada ação possível pelo sistema. Valor aceito:
    - números inteiro


 * **actionname**: Nome mostrado ao usuário. Por exemplo: luz sala. Valor aceito:
     - Strings


 * **type**: Tipos disponíveis para cada ação. Valor aceito:
   - Strings com os seguintes valores:
<<<<<<< HEAD
      - light
      - door
      - camera
      - plug
      - air
=======
    - light
    - door
    - camera
    - plug
    - air
>>>>>>> 9d18dae5f3d4d79d17ae131111325539ba80d94c


 * **do**: Ação propiamente dita, será utlilizado apenas quando uma ação for aplicado. Valor aceito:
     - Strings com os seguintes valores:
       - on
       - off
       - lock
       - unlock
       - block
