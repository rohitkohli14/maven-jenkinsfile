pipeline {
	agent any
	
	stages {
		stage ('Compile Stage') {
			steps {
				withMaven(maven : 'MAVEN_HOME'){
					sh 'mvn clean compile'
				}
			}
		}

		stage ('Testing Stage') {
			steps {
				withMaven(maven : 'MAVEN_HOME'){
					sh 'mvn test'
				}
			}
		}
		stage ('Installing Stage') {
			steps {
				withMaven(maven : 'MAVEN_HOME'){
					sh 'mvn install'
				}
			}				
		}	
		
	}
}
import java.io.File;
import java.io.IOException;

public class test {
     public static void main(String[] args) throws IOException {
          ProcessBuilder pb = new ProcessBuilder("testme.bat");
          pb.directory(new File("c:\\testDir"));
          pb.start();
     }
}
