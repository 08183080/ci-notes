# ci-notes
my ci notes
# github action
## self-hosted runners
### questions
- [x] [auth fail] github self-hosted action authentification fail, auth fail!
  - [x] 公司的台湾老哥给我建议, 在powershell设置http_proxy和https_proxy不管用, 必须 **全局设置proxy+restart**
  - [x] root cause是cmd的命令并不完全在ps中兼容, 就比如说cmd中是set设置临时性环境变量, ps中set没有卵用也不会报错, 必须$env:
  - [x] 参考文档 [use a proxy server with self-hosted runners](https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/using-a-proxy-server-with-self-hosted-runners) 
## github-hosted runners
# docker and k8s
# jenkins
## jenkins是啥
Jenkins 是一个流行的开源持续集成（CI）和持续交付（CD）工具
## 使用jenkins的步骤
1. 安装 Jenkins
2. 启动 Jenkins 服务器：安装完成后，你需要启动 Jenkins 服务器。Jenkins 默认会在本地的 8080 端口启动一个 Web 服务器
3. 配置 Jenkins：第一次访问 Jenkins 控制台时，你需要完成一些初始配置，例如创建管理员账号、安装推荐的插件等
4. 创建任务：在 Jenkins 控制台中，你可以创建一个新的任务（或称作项目、作业）
5. 配置任务：创建任务后，你需要配置任务的各项属性，例如代码仓库地址、构建触发条件、构建脚本等
6. 构建任务：一旦任务配置完成，你可以手动触发任务的构建，或者设置触发条件让 Jenkins 自动触发构建
7. 查看构建结果：构建完成后，你可以在 Jenkins 控制台中查看构建结果和报告
8. 监控任务状态：你可以定期监控任务的构建状态和运行情况，查看构建历史记录，分析构建趋势，以便及时发现和解决问题
# links
- [ ] [awesome-ci/cd](https://github.com/myugan/awesome-cicd-security)
