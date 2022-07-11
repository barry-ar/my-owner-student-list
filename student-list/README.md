# Student-list 
This repo is a simple application to list student with a webserver (PHP) and API (Flask)

## *Modifie index.php*
Modifie line 29:
`api_ip_or_name: app-v1` 
`port: 5000`
## *Test application*
Run command:
```
docker run --name NameContainer -p 80:5000 -v ${PWD}/student_age.json:data/student_age.json NameImages:Tags
```

## Run docker compose
````
docker-compose build 
docker-compose up -d
````

## *Open other terminal*
```
curl -u toto:python -X GET http://host_ip:port/pozos/api/v1.0/get_student_ages
```