# JUnit en Maven
JUnit con estructura Maven. Trabajo práctico 2 de la tercera evaluación.

# Test en Maven

- Verificamos si tenemos instalado Maven en nuestro computador.

        alumnado@A121PC12:~/gitlocal/JUnit-en-Maven$ mvn --version
        Apache Maven 3.3.9 (bb52d8502b132ec0a5a3f4c09453c07478323dc5; 2015-11-10T17:41:47+01:00)
        Maven home: /home/alumnado/Maven/apache-maven-3.3.9
        Java version: 1.8.0_131, vendor: Oracle Corporation
        Java home: /usr/lib/jvm/java-8-openjdk-amd64/jre
        Default locale: es_ES, platform encoding: UTF-8
        OS name: "linux", version: "4.4.0-78-generic", arch: "amd64", family: "unix"


- Realizamos git clone en nuestro espacio de trabajo.

        git clone [url_del_proyecto]
  
- Una vez estemos situados en la carpeta del proyecto, realizamos el siguiente comando:

        mvn package
    
- Nos devuelve el siguiente resultado:

          -------------------------------------------------------
           T E S T S
          -------------------------------------------------------
          Running Tp2_Ev3.JUnit.MathTest
          Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.098 sec

          Results :

          Tests run: 4, Failures: 0, Errors: 0, Skipped: 0

          [INFO] 
          [INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ JUnit ---
          [INFO] ------------------------------------------------------------------------
          [INFO] BUILD SUCCESS
          [INFO] ------------------------------------------------------------------------
          [INFO] Total time: 1.934 s
          [INFO] Finished at: 2017-05-18T11:03:10+02:00
          [INFO] Final Memory: 14M/167M
          [INFO] ------------------------------------------------------------------------

- Además, nos creará la carpeta /target, con el .jar compilado del proyecto.

          alumnado@A121PC12:~/gitlocal/JUnit-en-Maven$ ls -l
          total 52
          -rw-rw-r-- 1 alumnado alumnado 35141 may 17 11:14 LICENSE
          -rw-rw-r-- 1 alumnado alumnado   741 may 17 11:02 pom.xml
          -rw-rw-r-- 1 alumnado alumnado    92 may 17 11:14 README.md
          drwxrwxr-x 5 alumnado alumnado  4096 may 17 11:01 src
          drwxrwxr-x 8 alumnado alumnado  4096 may 18 11:06 target
          alumnado@A121PC12:~/gitlocal/JUnit-en-Maven$ 
