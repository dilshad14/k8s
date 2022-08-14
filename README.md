# k8s
samples, experiments around docker and k8s related

A.  **Database and Access tool**

1. **postgresql**

        PostegreSQL DB:  full fledged DB running in container and exposed inside k8s cluster only. following details are hardcoded in yaml file
   
            username: postgres
            password: mysecretpassword
            hostname to be used : pg-db-svc (since its only exposed into cluster via k8s service object)
            port: 5432

2.  **pg-admin4**
  
        pgAdmin 4 :  full fledged postgreSQL DB access UI tool, hosted on webserver. running inside container and exposed via k8s `NodePort` service object. server port is hardcoded in k8s manifest.
   
            open in browser URL : `http://localhost:30010`


B.  **Coming soon**