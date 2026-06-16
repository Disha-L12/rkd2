pipeline{
  agent any
  tools{
    gradle 'Gradle'
    jdk 'JDK'
    }
  stages{
  stage('checkout'){
  steps{
   git branch:'master' ,url:'https://github.com/Disha-L12/rkd2.git'
   }
   }
  stage('build'){
  steps{
  sh 'gradle build'
  }
  }
  
  stage('test'){
  steps{
   sh 'gradle test'
   }
   }
  stage('run'){
  steps{
  sh 'gradle run'
  }
  }
  }
post{
success{
echo 'success'
}
failure{
echo 'fail'
}
}}
