# Java and Eclipse Setup Guide (Windows 11)

This document provides step-by-step instructions to install Java (JDK) and Eclipse IDE on Windows 11.

---

## 1. Install Java (JDK)

### 1.1 Download JDK

Download the latest JDK from Oracle:

[https://www.oracle.com/java/technologies/downloads/](https://www.oracle.com/java/technologies/downloads/)

* Select Java SE (latest version)
* Download Windows x64 Installer (.exe)

---

### 1.2 Install JDK

1. Run the downloaded `.exe` file
2. Click Next → Next → Install
3. Default installation path:

   ```
   C:\Program Files\Java\jdk-xx
   ```
4. Click Close after installation

---

### 1.3 Set Environment Variables

#### Add JAVA_HOME

1. Press Windows + S
2. Search "Environment Variables"
3. Click "Edit the system environment variables"
4. Click "Environment Variables"
5. Under System Variables, click New

   Variable Name:

   ```
   JAVA_HOME
   ```

   Variable Value:

   ```
   C:\Program Files\Java\jdk-xx
   ```

---

#### Update PATH Variable

1. Select "Path" under System Variables
2. Click Edit → New
3. Add:

   ```
   %JAVA_HOME%\bin
   ```
4. Click OK on all windows

---

### 1.4 Verify Installation

Open Command Prompt and run:

```
java -version
javac -version
```

---

### 1.5 Test Java Program

Create a file named `Hello.java`:

```
class Hello {
    public static void main(String[] args) {
        System.out.println("Hello, Java");
    }
}
```

Compile and run:

```
javac Hello.java
java Hello
```

---

## 2. Install Eclipse IDE

### 2.1 Download Eclipse

Download Eclipse from Eclipse IDE:

[https://www.eclipse.org/downloads/](https://www.eclipse.org/downloads/)

Eclipse IDE for Enterprise Java and Web Developers (2025-12)
---

### 2.2 Run Installer

1. Open Eclipse Installer
2. Select "Eclipse IDE for Java Developers"

---

### 2.3 Configure Installation

* Choose installation directory (default is acceptable)
* Ensure JDK is detected
* Click Install
* Accept license agreement

---

### 2.4 Launch Eclipse

1. Click Launch
2. Select workspace directory, for example:

   ```
   C:\Users\YourName\eclipse-workspace
   ```

---

### 2.5 Create First Java Project

1. Click File → New → Java Project
2. Enter project name
3. Click Finish
4. Right-click project → New → Class
5. Add main method and run the program

---

## 3. Common Issues and Solutions

* javac not recognized
  Check PATH variable includes `%JAVA_HOME%\bin`

* Eclipse does not detect Java
  Verify JAVA_HOME is correctly set

* Incorrect version
  Install the latest JDK

---

## 4. Requirements

* Windows 11 (64-bit)
* Administrator access
* Internet connection

---

## 5. Optional Tools

* IntelliJ IDEA
* Visual Studio Code

---

## 6. Conclusion

Java and Eclipse IDE are successfully installed and configured. You can now begin developing Java applications.

---

