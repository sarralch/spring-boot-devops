# spring-boot-devops

Pipeline CI/CD Jenkins pour une application Spring Boot conteneurisée.

Git → Jenkins → Build & Test Maven → Docker Build → Docker Push → Déploiement MySQL → Déploiement backend-app → Vérification (docker ps / docker logs)

- Image : `backend-app:latest` (publiée sur `localhost:5000`)
- Conteneurs : `mysql`, `backend-app`
- Accès : http://192.168.33.10:8089/entreprise/all
