# Dubbo控制台

将dubbo-admin-ui项目打包放到dubbo-admin-server项目resource/static目录下

````
cd ./dubbo-admin-ui

npm run build

cp ./dubbo-admin-ui/target/dist/* /dubbo-admin-server/src/main/resource/static/

cd ./dubbo-admin-server

mvn package -DskipTests

cd ./docker-compose

docker build -t elijah/dubbo-admin:0.2.0 .

docker-compose up -d

````