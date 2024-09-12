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
    ![1](https://github.com/user-attachments/assets/8fe52255-96bd-421e-bf56-c3640a36f5fc)

5. **Open browser and login to Admin UI**
    ```sh
    <Public IP address>:943/admin
    ```

6. **Choose your OpenVPN plan and get activation key**
![Знімок екрана 2024-09-12 141628](https://github.com/user-attachments/assets/90444687-dd32-4e31-8f13-8ea9dfcda578)

7. **Create a user using Admin UI**
![Знімок екрана 2024-09-12 141932](https://github.com/user-attachments/assets/4c1d7838-30c8-42c4-9535-cf35ef7ad1ef)

8. **Login like a user and download OpenVPN for your platform and connect**
![3](https://github.com/user-attachments/assets/576b28ab-0b0f-4abc-9b21-10fb72015a88)

