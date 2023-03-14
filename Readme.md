# Project Name: My App
This is a Maven-based Java project for building a JAR file that includes a Python module. The JAR file can be executed and it will run a Python script included in the module.

### Project Structure
* `src/main/java`: This directory contains the source code of the Java application (Java Hello World Sample).
* `src/test/java`: This directory contains the unit test cases for the Java application.
* `src/main/python`: This directory contains the Python module and the script that will be executed ( Python Hello world and numpy Array Sample).
### Prerequisites
* JDK 1.8 or later.
* Apache Maven 3.5.4 or later.
* Python 3.7 or later.
* Numpy Python library installed.

### Build
To build the project, navigate to the project directory and execute the following command:

```mvn clean package```

The above command will build a JAR file named `my-app-1.0-SNAPSHOT.jar` in the `target` directory.

### Run
To run the application, navigate to the project directory and execute the following command:

```java -jar target/my-app-1.0-SNAPSHOT.jar```

The above command will execute the `hello.py` script included in the Python module.

### Testing
To run the unit tests, navigate to the project directory and execute the following command:


```mvn test```

### Maven Plugins

This project uses the following Maven plugins:

* `maven-compiler-plugin`: This plugin is used to compile the Java source code.
* `maven-jar-plugin`: This plugin is used to create a JAR file with the compiled Java classes and the Python module.
* `maven-enforcer-plugin`: This plugin is used to enforce the minimum Maven version required for building the project.
* `maven-antrun-plugin`: This plugin is used to copy the Python module files to the target directory.
* `exec-maven-plugin`: This plugin is used to execute Python scripts and install Numpy library.