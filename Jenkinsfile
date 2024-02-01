pipeline {
    // 定义 Jenkins Pipeline 工作流程
    agent {
        // 指定使用 Docker 容器作为运行环境
        docker {
            // 使用 maven:3-alpine 镜像
            image 'maven:3-alpine'
            // 挂载宿主机的 Maven 仓库到容器中，以便重用依赖
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages {
        // 定义构建阶段
        stage('Build') {
            steps {
                // 执行 Maven 构建命令，跳过测试，执行清理和打包
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}
