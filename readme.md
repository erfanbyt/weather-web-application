# weather webapp

This web application gets the city name from the user and and returns
* weather condition
* temperature
* how the weather feels like

### technologies used for this web app
* Flask 
* docker 

the inspiration for this web application was taken from [this](https://www.youtube.com/watch?v=jQjjqEjZK58). There are some modifications and also finally the application is containerized. 

## How to run
#### step 1
first of all make sure that you have docker installed on your system. 

#### step 2:
Go to the project directory and run the following command to create the docker image based on the dockerfile.

```bash 
docker build -t weather_app .
```

#### create and run the docker container
Running this command will run the app in a docker container and will expose it to `localhost:8000`

```bash 
docker run --rm -d -p 8000:8000 weather_app
```

This is the UI that for the app. 


![alt text](<Before running the app.png>)


![alt text](<Vancouver weather.png>)