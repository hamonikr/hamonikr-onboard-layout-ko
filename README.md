# Korean Keyboard Layout for onboard

한글 사용자를 위한 onboard 레이아웃 

![onboard-ko.png](./imgs/onboard-ko.png)
![onboard-ko2.png](./imgs/onboard-ko2.png)
![onboard-ko3.png](./imgs/onboard-ko3.png)
![onboard-ko4.png](./imgs/onboard-ko4.png)

# Install (HamoniKR-ME, HamoniKR-3.0)
```
sudo apt install hamonikr-onboard-layout-ko
```

# Install (Ubuntu, LinuMint, Other debian based Linux)
```
wget -O - http://apt.hamonikr.org/hamonikr.key | sudo apt-key add -
sudo bash -c "echo 'deb https://apt.hamonikr.org jin main upstream' > /etc/apt/sources.list.d/hamonikr-jin.list"
sudo apt-get update
sudo apt install hamonikr-onboard-layout-ko -y
```

# Install (Other Linux)

```
git clone https://github.com/hamonikr/hamonikr-onboard-layout-ko.git
cd hamonikr-onboard-layout-ko
sudo ./install
```

# Remove
```
sudo ./install remove
```

# Usage

Onboard Setting > Select Korean Layout

# License

[GPL3](./LICENSE)

