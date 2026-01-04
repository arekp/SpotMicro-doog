# SpotMicro-doog
instalacja raspery pi 4 
ubuntu 22.04 server
### Dodanie swap
# 1. Tworzenie pliku (2GB)
sudo fallocate -l 2G /swapfile

# 2. Nadanie uprawnień
sudo chmod 600 /swapfile

# 3. Formatowanie jako SWAP
sudo mkswap /swapfile

# 4. Włączenie pliku
sudo swapon /swapfile

# 5. Automatyczny start po restarcie (dodanie wpisu do fstab)
echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab

# 6. Weryfikacja
free -h

# Instalacja ROS2 
na podstawie strony [https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debs.html](instalacja)
w raperypi 4 instalujemy tylko
sudo apt install ros-humble-ros-base

na linux instalujemy
sudo apt install ros-humble-desktop
sudo apt install ros-dev-tools

## Podpiecia elektronika
schemat polaczen[https://gitlab.com/public-open-source/spotmicroai/electronics](Schemat poalczen)


