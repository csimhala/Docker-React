#Specify a base image
FROM node:alpine

#Install the dependencies
#If we doont mention the work directory, NPM will be installed in root directory and cause error
WORKDIR /mnt/c/Learning/Docker_and_Kubernetes/Examples/simpleweb
#Copy from local working directory to container working directory
COPY ./  ./ 
#Copy ./package.json ./  --> Copy if the change is only in package.json which will not run all the dependencies again
RUN npm install

#Default Command
CMD ["npm", "start"]