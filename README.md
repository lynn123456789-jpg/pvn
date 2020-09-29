# The neuroendocrine stress response at single-cell resolution. (Lopez et al., 2020)

> scRNA-seq analyses

***INSERT ANOTHER GRAPHIC HERE***

[![INSERT YOUR GRAPHIC HERE](http://i.imgur.com/dt8AUb6.png)]()

- Most people will glance at your `README`, *maybe* star it, and leave
- Ergo, people should understand instantly what your project is about based on your repo

> Tips

- HAVE WHITE SPACE
- MAKE IT PRETTY
- GIFS ARE REALLY COOL

> GIF Tools

- Use <a href="http://recordit.co/" target="_blank">**Recordit**</a> to create quicks screencasts of your desktop and export them as `GIF`s.
- For terminal sessions, there's <a href="https://github.com/chjj/ttystudio" target="_blank">**ttystudio**</a> which also supports exporting `GIF`s.


## Structure
HPA_reproducibility
|-- README.md
|-- code
|   `-- mast_scripts.py
|-- docker
|   |-- Dockerfile
|   `-- python-packages.txt
`-- notebooks
    |-- adrenal
    |   |-- 01-preprocessing.ipynb
    |   |-- 02-visualization.ipynb
    |   |-- 03-DE.ipynb
    |   `-- 04-ambient.ipynb
    |-- pituitary
    |   |-- 01-preprocessing.ipynb
    |   |-- 02-visualization.ipynb
    |   |-- 03-DE.ipynb
    |   `-- 04-ambient.ipynb
    |-- pvn
    |   |-- 01-preprocessing.ipynb
    |   |-- 02-visualization.ipynb
    |   |-- 03-DE.ipynb
    |   `-- 04-ambient.ipynb
    |-- rep_plots
    |   |-- main.ipynb
    |   `-- supplementary.ipynb
    `-- rep_tables
        `-- tables.ipynb

## Installation

We provide a Dockerfile with all the packages required to run the analyses. To build the Docker image use the command:
```shell
$ docker build docker -t hpa:latest
```

After the image is compiled, you can run it interactively using:

```shell
$  docker run --interactive --tty --name hpa --publish 8888:8888 --volume $HOME:/root/host_home --workdir /root hpa:latest  /bin/bash
```

This will start a container, in order to start a JupyterLab session use the alias:

```shell
$ jl
```

## Support

Reach out to me at one of the following places!

- Website at <a href="http://fvcproductions.com" target="_blank">`fvcproductions.com`</a>
- Twitter at <a href="http://twitter.com/fvcproductions" target="_blank">`@fvcproductions`</a>
- Insert more social links here.


## License

[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

- **[MIT license](http://opensource.org/licenses/mit-license.php)**
- Copyright 2015 © <a href="http://fvcproductions.com" target="_blank">FVCproductions</a>.
