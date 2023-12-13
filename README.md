# ML Python Flask of Mobile Programming Final Project Repository
This repository is used to fulfill Mobile Programming Final Project.
We utilize pretrained Deep Learning MobileNet V3 Small for Extracting Feature and predicting with Custom Model with 5 Dense Layer

## This application built with
* Flask
* Tensorflow

## Collaborator of This Project
* Muhammad Afdal Abdallah 50252012163
* Ingwer Ludwig 5025201259

# Getting Started
1. Clone repository following this command
    ```
    git clone https://github.com/ingwerludwig/ml-fp-ppb.git
    ```
2. Install python3 (>3.9 or latest)
3. Install pip (>18.1 or latest)
4. Install requirements.txt (prod-requirement.txt is for non MacOS Devices )
    ```
    pip install -r requirements.txt
    ```
    or
    ```
    pip install -r prod-requirements.txt
    ``` 
5. Start the WSGI Server for Running Python Flask App
    ```
     gunicorn --timeout 120 --bind 127.0.0.1:8000 app:app
    ```

6. (OPTIONAL) You can use PM2 library as process manager to auto restarting WSGI Server if it crash or down to maintain high availability
    ```
    npm install pm2 -g 
    ```
    then
    ```
    pm2 start "gunicorn --timeout 120 --bind 127.0.0.1:8000 app:app"
    ```
7. Test the API using `Postman` with `POST` Method, route `/predict` with image request body

## API Documentation
[API Documentation](https://myprivatepersonal.postman.co/workspace/PPB-FP-BACKEND~31694c8e-6ab1-4438-b8cb-7f1db18bf3f3/collection/26715144-29f8223e-2242-489d-8aba-a5db14e45dd0?action=share&creator=26715144&active-environment=26715144-a314cfaa-996d-493d-af8e-4323bd811da7)
or
You can export the postman collection from this repository
