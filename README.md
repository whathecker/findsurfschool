# findsurfschool
Public respository for findsurfschool.com 


## project overview
findsurfschool.com is my hobby project with a sub-goal to practice my technical skills and get experience with few technologies that I'm interested (mainly [kubernetes](https://kubernetes.io/)) 

website (unfinished): [link](https://www.findsurfschool.com)

This project use multi-repos and it consists of following 4 private repos:

1. surfschool-finder-k8s: Repository contains all kubernetes manifests

2. surfschool-finder-frontend: User interface of findsurfschool.com, it's a server-side rendered React application (NextJS)

3. surfschool-finder-content: Simple read only API written in NodeJS, it powers search functionality and surf school details

4. surfschool-finder-lead: TypeScript application to process the form request. the [API](https://api.findsurfschool.com/leadservice/api-docs/) talks to the GCloud function that sends an email to my Gmail account by impersonating myself. Architecture of the application is designed based on [Clean Architecture by Uncle Bob](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)


## infrastucture
The project is deployed on Google Kubernetes Engine. CloudFunction and other GCP services are used for SSL certificate, document storage, DNS..etc

## CI/CD
Each repository has its own CI/CD pipeline (GitHub Action), thus each service can be independently released

