# reinstall

## Content
- [Anaconda](#anaconda)
- [SSH](#ssh)
- [Snap](#snap)
- [Firefox](#firefox)
- [VPN](#vpn)
- [Deep Learning Machine](https://medium.com/@aragalie/build-your-own-top-spec-remote-access-machine-learning-rig-a-very-detailed-assembly-and-dae0f4011a8f)


## Anaconda
* should update current modules

* Download installer from [website](https://www.anaconda.com/distribution/)
* `bash <<path to script>>` 

***

## SSH

* on host

`sudo apt install openssh-server`

`sudo service ssh status`

* on client for login without password ([source](http://www.linuxproblem.org/art_9.html))

`a@A:~> ssh-keygen -t rsa` without passphrase 

`a@A:~> ssh b@B mkdir -p .ssh`

`a@A:~> cat .ssh/id_rsa.pub | ssh b@B 'cat >> .ssh/authorized_keys'`



***

## Snap

`sudo apt update`

`sudo apt install snapd`

`sudo snap install pycharm-professional --classic && sudo snap install telegram-desktop && sudo snap install youtube-dl && sudo snap install snap-store && sudo snap install spotify && sudo snap install vlc && sudo snap install code --classic`

***

## FireFox

* Bei Firefox Synchro anmelden

* Set normal Firefox scrolling speed
   * about:config
   * mousewheel.min_line_scroll_amount from 5 to 60

* Firefox Anpassen
   * turn off Titleleiste
   * Addons ins Überhangmenü verschieben

***

## VPN

* Download alpha-centauri-a.opvn from ssh://julians.cloud/root

`sudo apt install openvpn network-manager-openvpn`

`sudo systemctl restart network-manager`

* import downloaded file from above

* open `nm-connection-editor`
   * select typical internet connection
   * check the box "Automatically connect to VPN" and select your VPN
   
### Resources
* [Setting up deep learning machine](https://medium.com/@IsaacJK/setting-up-a-ubuntu-18-04-1-lts-system-for-deep-learning-and-scientific-computing-fab19f7ca39d)
* [Improve CPU Performance for DL](https://towardsdatascience.com/optimize-your-cpu-for-deep-learning-424a199d7a87)
