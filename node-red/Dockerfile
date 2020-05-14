FROM nodered/node-red:1.0.6

# copy node-red project files into place
COPY weather-dashboard/flows_linux.fritz.box.json /data/flows.json
COPY weather-dashboard/package.json /data/package.json
COPY settings.js /data/settings.js

RUN npm i node-red-contrib-influxdb@0.4.0
RUN npm i node-red-contrib-simple-gate@0.3.1
RUN npm i node-red-dashboard@2.22.1
RUN npm i node-red-node-ui-table@0.3.1
