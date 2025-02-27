# OpenXPKI

A simple way of getting familiar with OpenXPKI. A ready to use deployment with a default root CA certificate. SCEP enabled.

To start with your own deployment, clone the repository.
```
git clone https://github.com/mailsvb/openxpki.git
```

Either adapt the configuration found within the openxpki-config folder or simply start the docker containers by running
```
docker compose up -d
```

After the initial deployment, run the following command to create the root CA certificates
```
docker exec -it openxpki-docker-openxpki-server-1 /bin/bash /etc/openxpki/contrib/sampleconfig.sh
```
