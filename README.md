# Unix-Memory-Increase
Increase memory size for production build for AngularJS and VueJS (Might be useful for other reasons/frameworks as well)

Run `sudo fallocate -l 4G /swapfile;  ls -lh /swapfile; sudo chmod 600 /swapfile; sudo mkswap /swapfile; sudo swapon /swapfile; sudo swapon -s;  free -m;
`

Then run `sudo vim /etc/fstab` then add this to the bottom of the file -> ` /swapfile   none    swap    sw    0   0`
