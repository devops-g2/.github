## Project overview
This project encompasses a forum like website along with an SQLite backend and API.
The website is written in React (jsx) and bundled with Vite. 

Both the website and the API are dockerized and deployed to Azure ACR in a kubernetes cluster however we were not able to 
configure it in a way that the external IP and ports listen outside of the container before running out of free credits.. :(.

Building and running the images locally however, works!

The website and API are built and pushed using:
* docker build -t <image-name>:<tag> .
* docker push <image-name>:<tag>

We then apply our kubernets manifests from the prodeploy repository:
* kubectl apply -f deployment-<resource>.yml

To run locally and expose ports run:
* docker run -p <port>:<port> <image-name>

Monitoring and logging using Grafana, traefik, for the website and API is online meaning the services are healthy and deployed successfully, we just cant make requests to it.

## Github (gruppmedlemmar/githubalias):

 - Real name: Vanisha - Github name: [vanishah30](https://github.com/vanishah30)
 - Real name: Kevin Sundberg - Github name: [Dueweb](https://github.com/DueWeb) 
 - Real name: Hampus  - Github name: [QAsRevenge](https://github.com/QAsRevenge)
 - Real name: Emanuel - Github name: [emanueljg](https://github.com/emanueljg)
 - Real name: Sarmand - Github name: [Sarmand](https://github.com/sarmandjundi)

