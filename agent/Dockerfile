FROM jetbrains/teamcity-agent

RUN apt-get update -y
RUN apt-get install build-essential -y

RUN curl -L "https://github.com/docker/compose/releases/download/1.24.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
RUN chmod +x /usr/local/bin/docker-compose

RUN sysctl -w vm.max_map_count=262144
