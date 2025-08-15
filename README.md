# Hello Java Maven

This is a simple Java project built with Maven, designed for Jenkins CI/CD practice.

## Project Structure

```
hello-java-maven/
 ├── pom.xml
 └── src/
     └── main/
         └── java/
             └── HelloWorld.java
```

## How to Build Locally

1. Ensure you have **Java 8+** and **Maven** installed.
2. Clone the repository:
   ```bash
   git clone https://github.com/your-username/hello-java-maven.git
   cd hello-java-maven
   ```
3. Build the project:
   ```bash
   mvn clean package
   ```
4. Run the program:
   ```bash
   java -cp target/hello-1.0.jar HelloWorld
   ```

## Running in Jenkins

1. Create a new Freestyle project.
2. Configure Git repository URL.
3. Add a build step: **Invoke top-level Maven targets**
4. Set Maven goals:
   ```
   clean package
   ```
5. Build and verify `BUILD SUCCESS` in console output.

## Output

When you run the program, it will print:

Hello, Jenkins + Maven!


```
Hello, Jenkins + Maven!
```
