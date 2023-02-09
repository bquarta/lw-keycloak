docker build -t quarta/keycloak .

docker run --name keycloak-opt -p 8443:8443 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quarta/keycloak start --optimized