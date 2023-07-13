# Step 3: Launch Pi-WRF

<script async id="asciicast-BhZcW5ATh10bJIbxEpYJpvAC6" src="https://asciinema.org/a/BhZcW5ATh10bJIbxEpYJpvAC6.js?speed=2&i=8"></script>

## 3.1 Download and install docker on your Raspberry pi

To use this application on your raspberry pi (or computer) you need to
have docker installed. You can install
docker by opening your terminal and running the command below:

```
curl -sSL https://get.docker.com| sh
```

Executing the command above installs the latest stable version of Docker CLI, Docker Engine, and their dependencies on your device.

Once Docker is installed, you need to start the Docker application to proceed to the next step.


## 3.2 Launch the application

After successfully installing docker, copy and paste the command below
into your terminal.

```
docker run -p 8888:8888 ncar/pi-wrf
```

Executing this command pulls the ncar/pi-wrf docker image and runs an instance of the Pi-WRF notebook as a container in a non-persistant state (any changes to the notebook will not be saved) on your device. 

For information on how to run and persit changes made in the notebook, please NCAR's [Pi-WRF Github](https://github.com/NCAR/pi-wrf) page.



## 3.3 Open the Notebook

After the Docker container starts, some URLs appears in the terminal. You will need to copy and paste the one of the URL that starts with _http://127.0.0.1:8888_ into your browser. 

Entering the URL will open a locally hosted instance of Jupyter Notebook. You should select the Pi-WRF.ipynb notebook which will open in a new tab. The notebook provides instructions for selecting the domain and the datetime range for the model which we will explore in the next step.