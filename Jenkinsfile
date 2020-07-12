pipeline {
  agent any
  stages {
    stage('GetSourceCode') {
      steps {
        git(url: 'https://github.com/Baran121/api-teamplate-raml-mulesoft-ps.git', branch: 'master', credentialsId: '24c91e1a302ca6a5276ab9897f6b1a759f0ab1c6')
      }
    }

    stage('BuildIt') {
      steps {
        sh 'sh "mvn clean package"'
      }
    }

  }
}