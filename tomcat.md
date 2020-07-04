### [HOME](https://krishna-waidande-dev.github.io/krishna-waidande.github.io/)

# Tomcat Installation

1. Download the latest version of Tomcat zip file from here >> [Get Apache](https://tomcat.apache.org/download-90.cgi)

2. Open the Terminal (Ctrl + Alt + T). 

3. Move the downloaded Tomcat build to location where you wanted to install Tomcat.

```
cd <target-dir-path>
mv ~/Downloads/apache-tomcat-9.0.36.zip .
unzip apache-tomcat-9.0.36.zip 
```

4. Rename the folder name to apache-tomcat. (this step is optional)
> sudo mv apache-tomcat-8.0.26/ apache-tomcat/

5. Next to start Tomcat run the below script located in $Tomcat/bin directory. 
> $Tomcat/bin/startup.sh

6. To access the Tomcat in browser. Hit URL as http://localhost:8080/. 

7. To stop Tomcat run the below script located in $Tomcat/bin directory.
> $Tomcat/bin/shutdown.sh
