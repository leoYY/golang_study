### Go 目录结构约定

- $GOPATH/bin 编译后的二进制 go install 
- $GOPATH/pkg 编译中间产物 go build
- $GOPATH/src 源代码

### go代码与github上开发的规范
搭建Go环境的时候会初始化**$GOPATH**路径，可以分两种方式：  
1. 所有Go代码项目放在同一**$GOPAT**路径下，go get 获取git路径到$GOPATH/src目录下github.com/XXXX/XXX/ 后面的路径为实际github.com/XXXX/XXX.git的clone结果  
2. 每个项目单独**$GOPATH**路径，在每个项目中touch install文件，创建目录 $GOPATH/src/github.com/XXXX/XXX/， git clone到该目录下