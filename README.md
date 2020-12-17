# findsurfschool
Public respository for findsurfschool.com

## project overview
findsurfschool.com is my hobby project with a sub-goal to practice my technical skills and gain experience with few technologies that I'm interested (mainly [kubernetes](https://kubernetes.io/)) 

website: [link](https://www.findsurfschool.com)

This project use multi-repos and it consists of following 4 private repos:

1. surfschool-finder-k8s: repository contains all kubernetes manifests

2. surfschool-finder-frontend: user interface of findsurfschool.com, it's a server-side rendered React application (NextJS)

3. surfschool-finder-content: simple read only API written in NodeJS, it powers search functionality and surf school details

4. surfschool-finder-lead: TypeScript application to process the form request. the [API](https://api.findsurfschool.com/leadservice/api-docs/) talks to the GCloud function that sends an eamil to my Gmail account by impersonating myself. architecture of the application is designed based on [Clean Architecture style by Uncle Bob](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)




