FROM node:16
WORKDIR /app
RUN echo "Cloning UI...."
RUN git clone https://github.com/mohit000001/Node-Express-CRUD-APP.git
RUN echo "Cloning Done."
WORKDIR /app/Node-Express-CRUD-APP
RUN echo "Installing Dependencies...."
RUN npm install
RUN echo "Dependencies Done."
RUN echo "Installing Global Packages...."
RUN npm install --global nodemon
RUN npm install typescript -g
RUN echo "Global Packages Installation Done."
EXPOSE 9000
RUN echo "Starting Server...."
CMD ["npm", "start"] 