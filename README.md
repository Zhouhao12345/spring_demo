1. init environment

no_proxy=get.sdkman.io curl -s 'https://get.sdkman.io' | bash

echo 'export SDKMAN_DIR="/home/zhouhao/.sdkman" 
[[ -s "/home/zhouhao/.sdkman/bin/sdkman-init.sh" ]] && source "/home/zhouhao/.sdkman/bin/sdkman-init.sh"' >> ~/.zshrc

sdk install java 11.0.2-open

sdk install gradle 5.4.1

sdk install springboot 

sdk use java 11.0.2-open

gradle bootRun

2. run project

vi build.gradle & implementation 'org.springframework.boot:spring-boot-starter-web'
