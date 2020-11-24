>## 这是一个基于SpringCloud的微服务架构项目

>## 部署须知
1. 导入db目录下数据库文件到自己的MySQL服务器
2. 修改配置环境（xxx-service/src/main/resources/application.yml，active值决定启用环境配置文件）
3. 修改连接数据库配置（xxx-service/src/main/resources/application-fat.yml）
4. 修改前端页面连接网关地址（portal-service/src/main/resources/static/js/productList.js和orderList.js）
5. 服务启动顺序：eureka -> mysql -> product,stock,order -> gateway -> portal

>##注意：
打包是针对每个微微服务的，里面有3个微服务，每个微服务里面的pom.xml文件里面的依懒关糸目前还没有处理好；所以里面采用了一个全局的pom.xml文件进行打包
   
