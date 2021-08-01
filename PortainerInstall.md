# Portainer Install

## About

___"Portainer is a universal container management toolset that works with all of the major orchestration platforms - Kubernetes, Docker and Azure ACI. It helps organizations speed up the adoption of containers by removing the need for users to know any platform-specific code. <br/> <br/>
Portainer Business is built on our open source foundation, which has more than 500,000 users world wide. Portainer Business is fully featured, fully supported and proven to help organizations adopt containers quickly and easily. <br/> <br/>
If you're just starting out on your container journey or you're looking to speed up adoption of containers inside your organization then you're in the right place."___

## 1. Install Portainer

### 1.1 Creaate Volume to Portainer

```sh
docker volume create portainer_data
```

### 1.2 Install Portainer in volume and Run

```sh
docker run -d -p 8000:8000 -p 9000:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer
```

#### ; More docs: [Portainer.io - Install](https://documentation.portainer.io/v2.0/deploy/ceinstalldocker/)

## 2. Acess

[localhost:9000](http://localhost:9000)

### 2.1 Make initial creds setup

![Set Password Admin](https://documentation.portainer.io/v2.0/deploy/assets/initial-1.png)

Now you should be seeing something like this:

![Home](https://i.imgur.com/XBPKwPI.png)

## 3. It's done

#### ; [Portainer.io - Docs](https://documentation.portainer.io/)

## Made by

<p align="center">
  <br />
  ZauJulio ❤️
  <br />
</p>
