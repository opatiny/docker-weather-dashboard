FROM nodered/node-red:1.0.6

# copy node-red project files into place
COPY weather-bot/flow.json /data/flows.json
COPY weather-bot/flow_cred.json /data/flows_cred.json
COPY weather-bot/package.json /data/package.json
COPY settings.js /data/settings.js

RUN npm i node-red-contrib-influxdb@0.4.0
RUN npm i node-red-contrib-simple-gate@0.3.1
RUN npm i node-red-dashboard@2.22.1
RUN npm i node-red-node-ui-table@0.3.1
