pipeline {
    // 定义 Jenkins Pipeline 工作流程
    agent any
    stages {
        // 定义构建阶段
        stage('Build') {
            steps {
                sh '''cd /root/temp'
                    pwd
                    !在/root/temp创建一个文件，文件名为test-日期-小时-分钟-秒数
                    touch test-`date +%Y%m%d%H%M%S`.txt
                    '''
               }
        }
    }
}
