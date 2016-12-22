# 目的#
 
实验gRPC
	
# 步骤 #

**STEP1.工程构建**
	
	1.1.将pb文件编译成java文件
	$ ./gradlew generateProto

	1.2.生成eclipse工程，在eclipse中调试
	$ ./gradlew eclipse
	修改工程文件.classpath
		<classpathentry kind="src" path="build/generated/source/proto/main/java"/>
		<classpathentry kind="src" path="build/generated/source/proto/main/grpc"/>
	(最后一公里没有跳过)
	
**STEP2.debug 运行**
	
	2.1.运行helloWorldServer
	io.grpc.examples.helloworld.HelloWorldServer

	2.2.运行helloWorldClient
	io.grpc.examples.helloworld.HelloWorldClient
	
**STEP3.打包运行**

	3.1.编译打包
	$ ./gradlew installDist

	3.2.运行server
	$ ./build/install/examples/bin/hello-world-server

	3.3.运行client
	$ ./build/install/examples/bin/hello-world-client

# reference #
	
	http://www.grpc.io/docs/quickstart/java.html
	https://github.com/grpc/grpc-java
	https://www.zhihu.com/question/30027669/answer/70596887
