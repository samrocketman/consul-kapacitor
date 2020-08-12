# Consul Kapacitor

This demo shows an example of Kapacitor using consul for service discovery.

This is a companion project for
https://github.com/samrocketman/docker-compose-ha-consul-vault-ui

This assumes you have cloned this repository and
docker-compose-ha-consul-vault-ui to `${HOME}/git/github`.

docker-compose-ha-consul-vault-ui must be started before this project and be
healthy.

# Order of operations

1. Bootstrap [consul-influxdb][consul-influxdb]
2. Bootstrap [consul-kapacitor][consul-kapacitor] (this project)
3. Bootstrap [consul-chronograf][consul-chronograf]

# Bootstrapping this project

Simply run the following docker command.  It will register with consul
automatically.

    docker-compose up -d

[consul-chronograf]: https://github.com/samrocketman/consul-chronograf
[consul-influxdb]: https://github.com/samrocketman/consul-influxdb
[consul-kapacitor]: https://github.com/samrocketman/consul-kapacitor
