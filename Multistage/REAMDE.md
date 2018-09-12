# Multistageexample

Beide Images bauen 
und anschließend die
Größe der erbauten Images beider Dockerfiles vergleichen.


Bau des klassischen Dockerimages:

~~~
docker build -t golang1 .
~~~

Bau mit dem Multistagebuild:


~~~
docker build -t golang2 -f Dockerfile-multi  .
~~~
