pipeline {
    // 定义 Jenkins Pipeline 工作流程
    agent any
    stages {
        // 定义构建阶段
        stage('Build') {
            steps {
                sh 'cd /root/temp'
                sh 'pwd'
                // 执行 Maven 构建命令，跳过测试，执行清理和打包
            }
        }
    }
}
