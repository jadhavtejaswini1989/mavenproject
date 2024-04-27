pipeline
{
agent any
stages
{
 stage('scm checkout: download code from github')
 {steps { git branch: 'master', url: 'https://github.com/jadhavtejaswini1989/mavenproject.git'  }}


 stage('execute unit test framework')
 {steps {withMaven(globalMavenSettingsConfig: '', jdk: 'java_Home', maven: 'MAVEN_HOME', mavenSettingsConfig: '', traceability: true) {
    sh 'mvn test'
} } }

   }
}
