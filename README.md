# Infrastructure as Code With Observability

## Ruby install
Use [rv](https://github.com/spinel-coop/rv) to install ruby. E.g.:
```shell
rv ruby install 3.3.10
```

## R10k install
Use the following to install [r10k](https://github.com/puppetlabs/r10k):
```shell
cd openvox-code
gem cleanup
bundle config set path vendor/bundle
bundle install
```

## Module dependencies
Use the following to install Puppet module dependencies:
```shell
cd openvox-code && bundle exec r10k puppetfile install
```

## Start
Use the following docker command:
```shell
docker compose up -d
```

## Teardown
Use the following commands to teardown:
```shell
docker compose down --volumes
rm -rf openvoxserver-ca openvoxserver-ssl
```
