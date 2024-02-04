# select the base image to run
#  we want to run  Javascript file. so we can use the node runtime from the dockerHub
FROM node:20-alpine
# next we want to set the working directory. This is the directory commands will be run.
WORKDIR /app
#  this will copy the corrent directory to the docker image. first dot is the current directory on our machine, second dot is the path to the current direcrory with in the container.
COPY . .
#  we have to specify the command to run the app
CMD node hello.js

#  now docker file work is done. let's move into the folder docker file is located.
#  run this command -> `docker build -t hello-docker .`

# `-t` is optional, if no tag is provided, it defaults to the latest tag
#  and finally the path to the docker file

#  now we have the image.
# let's run or containerize it to see what happens `docker run hello-docker` (when u can see the console log)

#  if u go to docker desktop open that container and navigate inside of the 'files' u can see our file 'app'

#  if u open up the application in shell mode. `docker run -it hello-docker sh`
#  this put us directly within the operating system and the you can simply run `node hello.js` to see the same outpu.
#  we can publish the images created on Docker (This will be tying next steps)