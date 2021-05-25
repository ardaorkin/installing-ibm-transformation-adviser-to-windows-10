# HOW TO INSTALL IBM TRANSFORMATION ADVISER (WINDOWS 10 STEPS)
## Requirements
- IBM ID (you must be logged in)
- IBM Installation Manager
- Docker Engine (Docker Desktop App) in WSL 2 mode

## Installing IBM Installation Manager

- Create a directory like C:\IBM\WebSphere\Liberty in your machine where Installation Manager will be installed.
- Open [IBM Fix Central](https://www.ibm.com/support/fixcentral/swg/selectFixes?parent=ibm~Rational&product=ibm/Rational/IBM+Installation+Manager&function=all).
- Select the file which have the explanation “IBM Installation Manager Install Kit for all Windows versions supported by version 1.9.1.5”.
- Click Continue.
- In next page, click Download using your browser (HTTPS) option.
- Click Continue
- In next page, download the .zip file by clicking on it
- Save the file and extact it anywhere on the machine.
- Then run install.exe script which is in the extracted directory.
- When you face with the question about where to install the files in the installation process, select the C:\IBM\WepShpere\Liberty path.

## Installing Transformation Adviser
- Create a directory like C:\Users\ta_local\dockerCompose
- Share the directory everyone (you can follow the steps explained [here](https://www.windowscentral.com/how-share-files-and-printers-without-homegroup-windows-10)).
- Download necessarry files to the directory created just now, from [here](https://www.ibm.com/account/reg/signup?formid=urx-38642).
- Open Command Prompt or Powershell ISE (I recommend), go to the directory where you downloaded the files and run these commands respectively:
```shell
> docker-compose pull
> docker-compose up –d
```

Finally open http://localhost:3000 in a browser to be ensure that everything is working fine.
