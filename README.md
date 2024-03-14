# ci-notes
my ci notes
# github action
## self-hosted runners
### questions
- [x] [auth fail] github self-hosted action authentification fail, auth fail!
  - [x] 公司的台湾老哥给我建议, 在powershell设置http_proxy和https_proxy不管用, 必须 **全局设置proxy+restart**
  - [x] root cause是cmd的命令并不完全在ps中兼容, 就比如说cmd中是set设置临时性环境变量, ps中set没有卵用也不会报错, 必须$env:
## github-hosted runners
# docker and k8s
# links
- [ ] [awesome-ci/cd](https://github.com/myugan/awesome-cicd-security)

