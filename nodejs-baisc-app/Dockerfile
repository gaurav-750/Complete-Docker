FROM node

# create app directory in container
WORKDIR /app
#* now, all the subseq.commands will be in /app dir

# copy all files from current directory to /app in container

COPY package.json /app/

RUN npm install


COPY . /app/



# the container will listen on port 8080
EXPOSE 8080


# we want this command to run only when we run the container,
# not when the image is created

CMD ["node", "server.js"]


