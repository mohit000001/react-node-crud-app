FROM node:16
WORKDIR /app
RUN echo "Cloning UI...."
RUN git clone https://github.com/mohit000001/Crud-App-Frontend-React.git
RUN echo "Cloning Done."
WORKDIR /app/Crud-App-Frontend-React
RUN echo "Installing dependencies...."
RUN npm install
RUN echo "Dependencies Done."
RUN echo "Creating Production Build...."
RUN npm run build
RUN echo "Production Build Created."
RUN echo "Starting Server...."
RUN npm install -g serve
EXPOSE 80
RUN serve -s build -l 80
RUN echo "Server Setup Done."
