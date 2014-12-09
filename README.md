Fix error Ubuntu 14.04 command
============
- Error repo
```
sudo -i
apt-get clean
cd /var/lib/apt
mv lists lists.old
mkdir -p lists/partial
apt-get clean
apt-get update
```

- Hash sum miss
```
sudo rm /var/lib/apt/lists/*
sudo apt-get update
```
