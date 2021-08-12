# playground
a collection of **volatile** pre-built development playgrounds in docker containers 


## add your user to the docker group ##
``` sudo usermod -aG docker $(whoami) ```
then logout and back in again

## chmod the script ##
```sudo chmod +x ./playground ```

## launching a container ##

to launch a container you specify the container type - which can be found in `./containers/` - and the name of the container 

 to createa an ubuntu container called 1 you would run the following: 

``` ./playground ubuntu 1 ```

you will then see it spawn a docker container , update it with apt and install some basic utilities.

## more commands ##

./playground list                       ->   will list available images
./playground delete [container tag]     ->   will remove a playground
./playground search [grep thing]        ->   will grep the listed containers

## why? ##
we've all wanted to try something out in a fresh environment quickly before and this provides the perfect environment to try things out
it will allow for you to be able to quickly create containers with the tools you need to test your theories.

## additions ##
you can add your own containers to `./containers` but if they use docker-compose an edit of the script maybe needed

## //TODO ##
actually like fix input so they can't enter anything 
it's case sensitive 

