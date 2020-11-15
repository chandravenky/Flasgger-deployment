# Flasgger-deployment using Docker
Deploy risk classifier using Flasgger on local network using docker container

Make sure python is added to your PATH</b>

<b>Step 1: Open Anaconda Prompt<br></b>
Navigate to the folder

<b>Step 2: Create new environment<br></b>
python -m venv myflasggerapp_env

<b>Step 3: Activate the environment<br></b>
myflasggerapp_env\Scripts\activate.bat<br>
For macOS: source myflasggerapp_env/bin/activate

<b>Step 4: Install requirements<br></b>
pip install -r requirements.txt

<b>Step 5: Initialize docker - Check if you have docker<br></b>
docker

<b>Step 6: Build docker image<br></b>
docker build -t flasgger_api .

<b>Step 7: Check if you have docker image running<br></b>
docker images

<b>Step 8: Run the image<br></b>
docker run -p 5000:5000 flasgger_api

At this step, you can open another instance of Anaconda prompt and use docker ps command to check your container

<b>Step 9: Execute requests on http://localhost:5000/apidocs/<br></b>

<b>Note :</b> If you are using Docker Toolbox: Go to the ip on which your docker toolbox is configured




