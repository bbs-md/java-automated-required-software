
# Automated tests

## Installing Required Software

  - Intelij IDEA - https://www.jetbrains.com/ru-ru/idea/download/#section=windows or https://www.jetbrains.com/ru-ru/idea/download/download-thanks.html?platform=windows&code=IIC

  - JDK & JRE - https://www.oracle.com/java/technologies/downloads/ or https://download.oracle.com/java/21/latest/jdk-21_windows-x64_bin.msi

  - Maven - https://maven.apache.org/download.cgi or https://dlcdn.apache.org/maven/maven-3/3.9.9/binaries/apache-maven-3.9.9-bin.zip

  - Chrome driver - https://chromedriver.chromium.org/downloads or https://storage.googleapis.com/chrome-for-testing-public/129.0.6668.100/win64/chromedriver-win64.zip
    
  - Firefox - https://github.com/mozilla/geckodriver/releases or https://github.com/mozilla/geckodriver/releases/download/v0.34.0/geckodriver-v0.34.0-win32.zip

  - Git - https://git-scm.com/downloads/win

## Setting system environment variables in `Windows` OS

- Open `PowerShell` as Administrator and run commands

```
[Environment]::SetEnvironmentVariable("JAVA_HOME", "C:\Program Files\Java\jdk-14.0.2", "Machine")
[Environment]::SetEnvironmentVariable("MAVEN_HOME", "C:\Program Files\apache-maven-3.8.6", "Machine")
[Environment]::SetEnvironmentVariable("Path", $Env:Path + ';' + $Env:JAVA_HOME + '\bin', "Machine")
[Environment]::SetEnvironmentVariable("Path", $Env:Path + ';' + $Env:MAVEN_HOME + '\bin', "Machine")
```

- Check system variable. Open new `PowerShell` and run commands

```
echo $Env:JAVA_HOME
echo $Env:MAVEN_HOME
echo $Env:Path
```

![system_v](./images/system_v.png)

## Environment versions (this is just an example)

 - java and maven
  
![java](./images/java_version.png)

 - IntellijIdea
  
![idea](./images/idea_version.png)

 - chrome

![chrome](./images/chrome_version.png)

 - firefox

![firefox](./images/firefox_version.png)


  - WebDriverManager - https://bonigarcia.dev/webdrivermanager/#driver-management