``` this is the infra diagram ```
![Screenshot 2024-05-03 223700](https://github.com/Coding-warrior/kubernetes-mongodb-and-mongo-express/assets/60193256/75091350-5b33-4503-9fe1-356f7f85f491)

``` first create secret by doing ```
`` kubectl apply -f secretsmongo.yml ``

```then create mongodb.yml , this will up the mongodb ```
``` kubectl apply -f mongodb.yml ```

```then create configmap.yml , for pointing mongo-express pod toward mongodb service ```
``` kubectl apply -f configmap.yml ```

```then create mongo-express.yml.yml , this will create mongo-express deployment ```
``` kubectl apply -f mongo-express.yml ```
