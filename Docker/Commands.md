docker pull nginx
docker pull busybox
docker pull centos:centos8.4.2105
docker run -t -d centos sh
docker exec -it 9412c473340569a70964b64ce4399e3c5b824405450267aadf30496aae68ee00 sh
docker volume create prosan-demo-0
docker volume ls
docker run -it -v prosan-demo-0:/shared-volume --name centos-volume-test centos
docker run -it -v prosan-demo-0:/shared-volume --name centos-volume-test2 centos
docker run  -it -p 8001:80  --name apache-port-test httpd sh
docker build -t prosan-class-demo -f centos-dockerfile .
docker login
docker tag f0d23536890a venkatdock7/centos-prosan-demo:v1
docker images
docker push venkatdock7/centos-prosan-demo:v1