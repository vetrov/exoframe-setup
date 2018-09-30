# exoframe-setup

## 1. Install docker

https://docs.docker.com/install/linux/docker-ce/ubuntu/

## 2. Setup user for exoframe
```
# create exoframe user
sudo adduser exoframe

# add user to sudoers
sudo usermod -aG sudo exoframe

# add user to docker group (to run without sudo)
sudo usermod -aG docker exoframe
```

## 3. Create config/ssh folders
```
# switch to exoframe user
su - exoframe

# create configs folder
mkdir .ssh

# create authorized_keys
touch .ssh/authorized_keys

# set permissions
chmod 700 .ssh
chmod 600 .ssh/authorized_keys
```
