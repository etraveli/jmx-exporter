# Prometheus JMX Exporter in a docker container.

## Info
From openjdk:jre-alpine (specific version but to avoid updating to much)

## Usage
`docker run -v [pathToYourConfig]:/opt/jmx_export/config/jmx_exporter.yml -P etraveli/jmx_exporter`

It's setup with CMD, since it Alping you can use sh if you want to inspect the container.

It's exposed on 9209 -P for auto map or -p "externalPort:9209".

And don't forget localhost is only the docker host i network mode host.
