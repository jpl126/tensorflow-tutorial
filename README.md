# Tensorflow tutorial

This is my playground with [tensorflow](https://www.tensorflow.org/) tutorials.  
All examples were done the jupyter lab in the [docker](https://www.docker.com/) 
container.

## Getting started

To start you need installed docker - see 
[this](https://docs.docker.com/install/linux/docker-ce/ubuntu/) 
installation guide.

You can use docker image from the Tensorflow website or use my image with 
jupyter lab and python 3 on board.

To start simply run following command:  
`docker run -it -u user --rm -v [YOUR LOCAL DIRECTORY WITH NOTEBOOKS]:/tf/notebooks -p 8888:8888  jacekplocharczyk/tensorflow:jupyter-lab  jupyter-lab --ip 0.0.0.0
`

This will allow you to use jupyter-lab in web browser at localhost address.  
Please note that you need to provide authentication token from the console output. 
 
Example:
```
jacek@jacek-Lenovo-Y50-70:~$ docker run -it -u user --rm -v $(realpath ~/Dokumenty/projects/tensorflow-tutorial):/tf/notebooks -p 8888:8888 jacekplocharczyk/tensorflow:jupyter-lab jupyter-lab --ip 0.0.0.0
[I 08:23:09.568 LabApp] Writing notebook server cookie secret to /home/user/.local/share/jupyter/runtime/notebook_cookie_secret
[I 08:23:09.802 LabApp] JupyterLab extension loaded from /usr/local/lib/python3.5/dist-packages/jupyterlab
[I 08:23:09.802 LabApp] JupyterLab application directory is /usr/local/share/jupyter/lab
[W 08:23:09.804 LabApp] JupyterLab server extension not enabled, manually loading...
[I 08:23:09.806 LabApp] JupyterLab extension loaded from /usr/local/lib/python3.5/dist-packages/jupyterlab
[I 08:23:09.806 LabApp] JupyterLab application directory is /usr/local/share/jupyter/lab
[I 08:23:09.807 LabApp] Serving notebooks from local directory: /tf
[I 08:23:09.807 LabApp] The Jupyter Notebook is running at:
[I 08:23:09.807 LabApp] http://(e03b8e333a1f or 127.0.0.1):8888/?token=3b2a11a36f82e261194f46c3cc61ca60d05277004a53a21b
[I 08:23:09.807 LabApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[W 08:23:09.810 LabApp] No web browser found: could not locate runnable browser.
[C 08:23:09.810 LabApp] 
    
    To access the notebook, open this file in a browser:
        file:///home/user/.local/share/jupyter/runtime/nbserver-1-open.html
    Or copy and paste one of these URLs:
        http://(e03b8e333a1f or 127.0.0.1):8888/?token=3b2a11a36f82e261194f46c3cc61ca60d05277004a53a21b
[W 08:23:10.279 LabApp] Clearing invalid/expired login cookie username-localhost-8888

```
