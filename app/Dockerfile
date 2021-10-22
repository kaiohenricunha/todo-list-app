# base image and linux alpine
FROM node:12-alpine

# installs some dependencies
RUN apk add --no-cache python g++ make

# setting the working directory
WORKDIR /app

# copy-pasting my app(and its dependencies) to the image i'm creating
COPY . .

# gets some more dependencies
RUN yarn install --production

# specifies the commands to run when starting a container
CMD ["node", "src/index.js"]