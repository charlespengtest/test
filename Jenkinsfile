pipeline {
  agent any
  stages {
    stage('检出') {
      steps {
        echo '检出'
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'b6d49509-3755-43f1-99b3-a73c22a53ef5', url: 'https://github.com/charlespeng7/PLTest']]])
        sleep 10
      }
    }
    stage('构建') {
      steps {
        echo '构建中...'
        sleep 10
      }
    }
    stage('测试') {
      steps {
        echo '单元测试中...'
        echo '单元测试完成.'
        sleep 10
      }
    }
    stage('部署') {
      steps {
        echo '部署中...'
        echo '部署完成'
      }
    }
  }
}
