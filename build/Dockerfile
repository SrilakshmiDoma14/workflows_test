FROM node:15.14.0
WORKDIR /app
COPY codebase/rdicidr-0.1.0 .
RUN npm install
RUN npm install prettier
RUN npm run prettier
RUN npm run build
RUN npm install -g serve@12.0.1
EXPOSE 5000
CMD ["serve", "-s","build"]