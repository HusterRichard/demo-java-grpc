# Ŀ��#
 
ʵ��gRPC
	
# ���� #

**STEP1.���̹���**
	
	1.1.��pb�ļ������java�ļ�
	$ ./gradlew generateProto

	1.2.����eclipse���̣���eclipse�е���
	$ ./gradlew eclipse
	�޸Ĺ����ļ�.classpath
		<classpathentry kind="src" path="build/generated/source/proto/main/java"/>
		<classpathentry kind="src" path="build/generated/source/proto/main/grpc"/>
	(���һ����û������)
	
**STEP2.debug ����**
	
	2.1.����helloWorldServer
	io.grpc.examples.helloworld.HelloWorldServer

	2.2.����helloWorldClient
	io.grpc.examples.helloworld.HelloWorldClient
	
**STEP3.�������**

	3.1.������
	$ ./gradlew installDist

	3.2.����server
	$ ./build/install/examples/bin/hello-world-server

	3.3.����client
	$ ./build/install/examples/bin/hello-world-client

# reference #
	
	http://www.grpc.io/docs/quickstart/java.html
	https://github.com/grpc/grpc-java
	https://www.zhihu.com/question/30027669/answer/70596887
