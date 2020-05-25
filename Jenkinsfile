pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        echo "Building"
      }
    }
    
    stage("test") {
      steps {
        echo "Testing"
      }
    }
    
    stage("deploy") {
      steps {
        echo "Deploy"
      }
    }
  }
  post {
    always {
      allure report: 'allure_reports', results: [[path: '/Users/kcheng/mypypi/b2b/demo/tests/functional/reports/my_allure_results/']]
}
