部署：

mvn package后将war copy到tomcat下


测试：

查一个记录：

http://localhost:8080/SpringRestExample-1.0.0-BUILD-SNAPSHOT/rest/emp/dummy

另一种方法查记录：
http://localhost:8080/SpringRestExample-1.0.0-BUILD-SNAPSHOT/rest/emp/9999


查所有记录：

http://localhost:8080/SpringRestExample-1.0.0-BUILD-SNAPSHOT/rest/emps  get all 


删除：

curl -X PUT -G --user-agent "Mozilla/4.73 [en] (X11; U; Linux 2.2.15" http://localhost:8080/SpringRestExample-1.0.0-BUILD-SNAPSHOT/rest/emp/delete/9999


查所有记录：
http://localhost:8080/SpringRestExample-1.0.0-BUILD-SNAPSHOT/rest/emps


增加一条记录：
curl -H "Content-Type: application/json" -X POST -d '{"name":"tom","id":"8888"}' http://localhost:8080/SpringRestExample-1.0.0-BUILD-SNAPSHOT/rest/emp/create


查所有记录：
http://localhost:8080/SpringRestExample-1.0.0-BUILD-SNAPSHOT/rest/emps

