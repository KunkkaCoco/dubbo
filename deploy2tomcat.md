

发布到tomcat：
    
    1.复制 dubbo-admin-xx.war 到 ${tomcat-home}/webapps 
        cp dubbo-admin-xx.war ${tomcat-home}/webapps 
    2.解压并重命名为ROOT  注意备份原ROOT文件。
         unzip dubbo-admin-2.4.1.war -d webapps/ROOT
    3.修改ROOT/WEB-INF/dubbo.properties 的注册地址
        vi webapps/ROOT/WEB-INF/dubbo.properties
        dubbo.registry.address=zookeeper://127.0.0.1:2181
        dubbo.admin.root.password=root
        dubbo.admin.guest.password=guest
