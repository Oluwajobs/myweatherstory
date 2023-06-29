# Step 3: Launch Pi-WRF

## 3.1 Download and install docker on your Raspberry pi

To use this application on your raspberry pi (or computer) you need to
have docker installed. If you haven’t already done so you can install
docker my opening a terminal and running the command below:

```
curl -sSL https://get.docker.com \| sh
```

## 3.2 Launch the application

After successfully installing docker, copy and paste the command below
into your terminal.

```
sudo docker run -it --rm --net=host -e DISPLAY -v
\$HOME/.Xauthority:/root/.Xauthority ncar/pi-wrf
```

When you enter the following command and execute it, Docker downloads
the file for you and then launches the application. If you close the
program, Docker will save the “file” so you do not have to download it
the next time you run the application.
