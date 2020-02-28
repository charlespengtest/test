pipeline {
  agent any
  stages {
    stage('检出') {
      steps {
        echo '检出'
      }
    }
    stage('构建') {
      steps {
        echo '构建中...'
      }
    }
    stage('测试') {
      steps {
        echo '单元测试中...'
        echo '单元测试完成.'
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
