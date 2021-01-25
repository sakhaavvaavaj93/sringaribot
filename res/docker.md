## sringaribot




#### The Easy Way [ 🐳 ]

Writing this again, since I have seen many users recommending **SUDO** to install Docker.
It is not recommended to use "sudo", while using Docker.
GNU/Linux Permissions are highly customisable, and it is generally not required to have "ROOT" permission, ~~unless you know what you are doing~~.
You can still install all the dependencies in your system [with ROOT permissions],
but please be aware of the potential issues when doing so. The installed packages
may conflict with the system package manager's installed packages, which can
cause trouble down the road and errors when upgrading conflicting packages.
**You have been warned.**

- **Install docker**: Follow the official docker [installation guide](https://docs.docker.com/engine/install/).

- **Install Docker-compose**: Follow the official composer [installation guide](https://docs.docker.com/compose/install/).

- **create CONFIG file**: 
  - ```wget https://raw.githubusercontent.com/sakhaavvaavaj93/sringaribot/master/sample_config.env -O config.env```
  - edit the file by removing the `#` in the required fields, and adding values.

- **downloading the sringaribot** `docker-compose` YAML file:
  - ```wget https://raw.githubusercontent.com/sakhaavvaavaj93/sringaribot/master/docker-compose.yml```

- **start the bot**: ```docker-compose up -d```

- The bot should be running now. Check logs with ```docker-compose logs -f```
