pipeline{
  agent any
  tools{
      maven 'Maven'
      jdk 'JDK'
}
  stages{
    stage('Checkout'){
        steps{
            echo 'Checkout'
            git branch:'master', url:'https://github.com/bitcse6c/1BI22CS152.git'
    }
}
  stage('Build'){
    steps{
          echo 'Build'
          sh 'mvn clean package'
  }
  }
stage('Test'){
  steps{
      echo 'Test'
      sh 'stage('Deploy War'){
  steps{
    echo 'Copied'
    sh 'sudo cp /target/MyMavenApp.war /opt/tomcat/webapps/'

}
}
}mvn test'
  }

    stage('Deploy'){
      steps{
        echo 'Deploy'
        sh 'sudo cp target/MyMavenApp.war /opt/tomcat/webapps'

}
    }
post{
  success{
    echo "Successfully Excuted"
}
  failure{
    echo "Failure "
}


}
}
