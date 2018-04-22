# RCMPhack


Readme file

Following this tutorial - https://blog.patricktriest.com/text-search-docker-elasticsearch/

To setup this search I had to do the following;

install docker
  https://docs.docker.com/install/
install docker compose
  https://docs.docker.com/compose/install/#install-composehttps://docs.docker.com/compose/install/#install-compose

  The setup in docker-compose.yml is pointing all ports to localhost.  Update ports here.
 - this file is also tying in the API, frontend and search containers.

 *note must use 'sudo docker-compose build' to build*
 *use 'sudo docker-compose up' to run as daemon, -d switch runs as background process*

Book mapping is defined here in server/connection.js

 **Here we are defining a mapping for the book index. An Elasticsearch index is roughly analogous to a SQL table or a MongoDB collection. Adding a mapping allows us to specify each field and datatype for the stored documents. Elasticsearch is schema-less, so we don't technically need to add a mapping, but doing so will give us more control over how the data is handled.**


Search functions (in search.js) are linked to API via /server/api.js -> note endpoints comment in app.js

Chart.js tutorial here -> https://alligator.io/vuejs/vue-chart-js/
