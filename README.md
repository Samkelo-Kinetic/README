# FUNCTIONAL-TESTING ON LOCAL-MACHINE ENVIRONMENT SETUP, UBUNTU OS. 

Following the steps below will ensure a smooth mobile functional-testing environment.


# TOOLS NEEDED IN SEQUENTIAL MANNER

 *java, jdk and jre
 *android studio
 *appium
 *appium doctor
 *pipenv
 *toolium
 *chromedriver
 *Genymotion(emulators)
 
install node.js without using sudo(poweruser)
  
  Download and install latest release of nodejs
  
  https://nodejs.org/download/release/latest/node-v11.14.0-linux-x64.tar.gz
 
# Install it under/usr/local
  
     *cd /usr/local tar --strip-components 1 -xzf /home/username/Downloads/node-v11.14.0-linux-64.tar.gz
 
On the terminal check the success of the installation by the following command
     
     * node -v
  
 
# Install Java, jdk and jre-

    * sudo apt-get update
    * sudo apt-get install default-jre
    * sudo apt-get install default-jdk
    //to install oracle jdk
    * sudo add-apt-repository ppa:webupd8team/java
    * sudo apt-get update
    * sudo apt-get install oracle-java8-installer
    
 #  Set JAVA HOME path
 
    //open bashrc file 
    * gedit ~/.bashrc
    * export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
    * export PATH=${PATH}:${JAVA_HOME}/bin
     //run following command to verify the path
    * echo $JAVA_HOME
    * echo $PATH
    
   Command to check if java is installed:
    
    * which java
    
# Download android studio and set the ANDROID HOME path
 
  To open android studio open terminal and install android android sdk
 
    * cd android-studio/bin ./studio.sh
    
   Once android sdk is installed, Set ANDROID HOME path using:
     
    * gedit /.bashrc
    * //add following lines at the end of the file and then save
    * export ANDROID_HOME=/home/user_name/Android/Sdk
    * export PATH=$PATH:/home/user_name/Android/Sdk/tools
    * export PATH=$PATH:/home/user_name/Android/Sdk/platform-tools
    
# Install appium globally
 
    * npm install -g appium
     
# Install appium-doctor to troubleshoot errors
 
    * npm install -g appium-doctor
    
    
 
 First cd into the project and follow the below step.
# Install python pipenv (preferrably 3.5.2)
 
    * pipenv install python3.5.2
    * To activate this project's virtualenv run,
       ~pipenv shell~
    *Alternatively, run a command inside the virtualenv with,
      pipenv run

# Install toolium

     * sudo -H pip install toolium
     * sudo -H pip install git+https://github.com/behave/behave
     
# Install chromedriver 

Your current directory should be "$HOME" as illustrated below:

cd "$HOME"
wget -O "chromedriver_linux64.zip" "https://chromedriver.storage.googleapis.com/2.37/chromedriver_linux64.zip"
unzip -o "chromedriver_linux64.zip"
sudo cp "chromedriver" "/usr/local/bin/chromedriver"
sudo chmod +x "/usr/local/bin/chromedriver"
rm -f "chromedriver"
rm -f "chromedriver_linux64.zip"

To ensure chromedriver is successfully installed check on the terminal with the below command:

    *which chromedriver

# Steps to install Genymotion (Android Emulator)
   
Step 1. Download Genymotion (Android Emulator) link:https://www.genymotion.com/fun-zone/

Step 2. Open terminal (ctrl+alt+t) and type below command to install virtualbox 

sudo apt-get install virtualbox

Step 3. Now go to location where you downloaded Genymotion and run below command

chmod +x genymotion-3.0.1_x-linux64.bin(check the version of genymotion you downloaded and replace 
"genymotion-3.0.1_x64.bin" with it.)

and after this

./genymotion-3.0.1_x-linux64.bin(your downloaded version)

Step 4. Open Genymotion and create virtual device first

Step 5. Select Android virtual device available to install from the list

Step 6. Install virtual device you prefer


Testing how to make a table in a readmefile

| Tables        | Are           | Cool   |
| ------------- |:-------------:| -----: |
| bonga         | sam           |xolani  |       
| kwennie       | darren        | rowan  |
| kids          | kids          | kids   |
 
Testing how to make a checklist in readmefile 
- [x] login feature--
- [x] register feature
- [ ] forms feature
- [ ] burns feature
- [x] ophathalmolgy feature


