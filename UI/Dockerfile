FROM node:16
WORKDIR /app
RUN echo "Cloning UI...."
RUN git clone https://github.com/mohit000001/Crud-App-Frontend-React.git
RUN echo "Cloning Done."
WORKDIR /app/Crud-App-Frontend-React
RUN echo "Installing dependencies...."
RUN npm install
RUN echo "Dependencies Done."
RUN echo "Starting Server...."
EXPOSE 80
RUN npm run prod-server
RUN echo "Server Setup Done."
