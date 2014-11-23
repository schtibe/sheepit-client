# SheepIt Render Farm Client

## Website

[SheepIt RenderFarm](https://www.sheepit-renderfarm.com)

## Overview

SheepIt Render Farm Client is an *Open Source* client for the distributed render farm "Sheep It".




## Compilation

You need Java 1.7, OpenJDK or Oracle are supported.
You also need ant.
To create the jar file, simply type "ant".

## Usage

Once you have a jar file you look at the usage by doing "java -jar bin/sheepit-client.jar --help".
When you are doing your development you can use a mirror of the main site who is specially made for demo/dev, it is localted at **http://www-demo.sheepit-renderfarm.com**

## Configuration file

You can specify a configuration file with the options from the command line. For example:


    java -jar bin/sheepit-client.jar -config settings



Inside the settings file:

    username=EXAMPLEUSER
	password=EXAMPLEPW
	verbose=true
	cache-dir=/tmp/
	compute-method=CPU_GPU
	cores=2
	gpu=CUDA_0
	server=https://www.sheepit-renderfarm.com
	request-time 2:00-8:30,17:00-23:00

Note that only the username and password are mandatory, the other options will fall back
to default if you don't specify them.
