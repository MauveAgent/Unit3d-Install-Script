<h1 align="center">UNIT3D Install Script Reborn</h1>

<h1 align="center">WE ARE NOT AFFILIATED WITH UNIT3D!</h1>

<p align="center"><b>WE (I) AM NOT AFFILIATED WITH UNIT3D IN ANY OFFICIAL CAPACITY. USAGE OF THIS SCRIPT IS AT YOUR OWN RISK & I OFFER NO PROMISES OR LIKEWISE IN TERMS OF COMPATABLITY, CONTINUED USAGE OVER TIME, OR PROMISES OF RISK FREE USE. PLEASE BE SURE TO SECURE / HARDEN YOUR SERVER AFTER INSTALLATION. WE ARE NOT RESPONSIBLE FOR ANY OR ALL DATA LOSS / CORRUPTION OR SIMILAR. ALL USERS OF THIS SCRIPT - ACCEPT ANY AND ALL LIABILITY AND RESPONSBILITY FOR IT'S USAGE. LIKEWISE, THIS IS AN UNOFFICIAL FORK. PLEASE DO NOT HARASS THE DEVELOPERS OF UNIT3D WITH ISSUES PERTAINING TO THIS SCRIPT. THEY ARE NOT OBLIGATED TO HELP YOU.</b></p>

</br>

<h1 align="center">NO SUPPORT NOTICE -- SOFTWARE PROVIDED AS-IS.</h1>

<p align="center"><b>WARNING: NO SUPPORT WILL BE GIVEN, IN ANY CAPACITY. THIS IS SIMPLY A PERSONAL TOOL I UPDATED FOR MY USAGE. I DO NOT HAVE THE TIME TO HELP WITH ISSUES & THIS IS PROVIDED AS-IS. THE UNIT3D PROJECT CHOSE TO REMOVE THEIR INSTALLER - AND WILL NOT PROVIDE SUPPORT TO MY KNOWLEDGE. DO NOT HARASS THEM.</b></p>

<h1 align="center">Manual Intervention Required Post Install!</h1>

<p align="center"><b>BE ADVISED: YOU WILL NEED TO BE COMFORTABLE WORKING FROM THE COMMAND LINE. YOU WILL NEED TO INSTALL SOFTWARE, EDIT CONFIGURATION FILES BY HAND, AND ADJUST ENVIRONMENT VARIABLES POST INSTALL. I HAVE NO DESIRE TO UPDATE THE SCRIPT FOR THOSE NEEDS, AND DON'T INTEND TO. - IF YOU DECIDE TO DO SO, PLEASE CONSIDER FORKING AND MAKING A PULL REQUEST FOR SOURCE CODE REVIEW.</b></p>



## FOR MANUAL POST-INSTALL INSTRUCTIONS SEE THE [WIKI](https://github.com/MauveAgent/Unit3d-Install-Script/wiki)

---

</br>

## FOR NEW INSTALLATIONS - FRESH SERVERS ONLY.

<p align="center"><b>NOTE: This only works for a fresh server with nothing on it but a new OS install!</b></p>

## This Repository
Un-Offical Installer for the [UNIT3D](https://github.com/HDInnovations/UNIT3D).

**Officially Supported OS's**
- Ubuntu 24.04 LTS (Noble Numbat)
- Ubuntu 22.04 LTS (Jammy Jellyfish)
- Ubuntu 20.04 LTS (Focal Fossa)

**To install run the following:** (and follow the instructions. must be a fresh deicated server with nothing on it besides supported OS. Also must have a proper valid domain pointing to your server IP via A RECORD and CNAME for www) - Google is your friend. 

```
sudo apt -y install git
git clone https://github.com/MauveAgent/Unit3d-Install-Script.git installer
cd installer
sudo ./install.sh
```

**NOTE: If you are running UNIT3D on a non HTTPS instance you MUST change the following configs.**
```
.env  <-- SESSION_SECURE_COOKIE must be set to false
config/secure-headers.php   <-- HTTP Strict Transport Security must be set to false
config/secure-headers.php   <-- Content Security Policy must be disabled
```
