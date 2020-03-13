# migracion
1) jboss_migration.yml
   - migracion de todos los configs y wars del viejo jboss al nuevo


2) jboss_start_service.yml
   - levantar todos los jboss con eap 7.2, el domain controller con jdk 11 y los slaves con jdk 8

3) jboss_upload_wars.yml
   - upload new wars to the jboss eap repo

4) server-group A

   4.1) jboss_undeploy_all.yml
        - undeploy all wars from server-group A

   4.2) jboss_start_service.yml
        - restart jboss eap with jdk 11

   4.3) jboss_deploy.yml
        - deploy new wars to server-group A 


5) repeat steps 4 for server-group B
