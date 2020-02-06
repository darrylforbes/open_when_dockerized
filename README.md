Open When Dockerized

    Version 2 of https://github.com/darrylforbes/open_when

    Improvements
        - Dockerized
        - More organized cloud infrastruture
        - Better coding practices

Planned Architecture

    EC2
        - Container 1: Django REST API served using Gunicorn
        - Container 2: NGINX
        - Container 3: Development postgres database
        - Container 4: Development react app

    RDS
        - Production postgres database

    S3
        - Production react app

Other Plans

    Create CI/CD pipeline

    Possibly replace NGINX with Traefik once static files are relocated too S3

    Enable HTTPS with LetsEncrypt (possibly switch to Traefik for built in SSL)
