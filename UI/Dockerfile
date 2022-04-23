FROM node:16
WORKDIR /app
RUN echo "Cloning UI...."
RUN git clone https://github.com/mohit000001/Crud-App-Frontend-React.git
RUN echo "Cloning Done."
RUN echo "Installing dependencies...."
RUN cd Crud-App-Frontend-React && npm install
RUN echo "Dependencies Done."
RUN echo "Creating Production Build...."
RUN npm run build
RUN echo "Build Created."
RUN echo "Installing Server...."
RUN npm install -g serve
RUN echo "Server Installed."
RUN echo "Starting Server...."
EXPOSE 80
RUN serve -s build -l 80
RUN echo "Server Setup Done."
