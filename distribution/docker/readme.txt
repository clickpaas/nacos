
mvn -Prelease-nacos -DskipTests -Dcheckstyle.skip=true clean install -Dmaven.test.skip

#打好的包拖入 https://file.devops.clickpaas.tech/software/

cd docker; make push