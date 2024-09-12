# Deployment Guide
1. **Clone this repository and use terraform configuration**
    ```sh
    terrafrom init
    terraform apply
    ```
## OpenVPN

1. **SSH log in to VM**
    ```sh
    ssh testadmin@<public_ip>
    ```

2. **Install updates and set the correct time**
    ```sh
    apt update
    apt upgrade
    apt install tzdata
    dpkg-reconfigure tzdata
    ```

3. **To install Access Server on your Linux server, run this command:**
    ```sh
    bash <(curl -fsS https://as-repository.openvpn.net/as/install.sh)
    ```

4. **Find your login and password to Admin UI.**
![image](https://github.com/user-attachments/assets/00caa2e5-827e-41c3-94bf-ed628c4f75fa)
![image](https://github.com/user-attachments/assets/36785e9d-428b-4f0b-abb8-3d8f550fbb36)
5. **Open browser and login to Admin UI**
    ```sh
    <Public IP address>:943/admin
    ```

6. **Choose your OpenVPN plan and get activation key**
![Знімок екрана 2024-09-12 141628](https://github.com/user-attachments/assets/90444687-dd32-4e31-8f13-8ea9dfcda578)

7. **Create a 2 user using Admin UI**
![image](https://github.com/user-attachments/assets/347b9394-99c7-4d9b-aded-f6f1e4c9f827)
![image](https://github.com/user-attachments/assets/7399bf77-6421-4988-b212-377d0b45c018)


8. **Login like a user and download OpenVPN for your platform and connect**
![image](https://github.com/user-attachments/assets/9a333f44-52bf-4448-aa7b-da374a4114f4)


