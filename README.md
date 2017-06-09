# s2jdbc-tutorial

1,在lib文件夹里追加postgre的jdbc包.
       如:postgresql-9.3-1100.jdbc4.jar
  
2,设定数据库联接
  /s2jdbc-tutorial/src/main/resources/jdbc.dicon
       修改内容:
  <component name="xaDataSource" class="org.seasar.extension.dbcp.impl.XADataSourceImpl">
		<property name="driverClassName">"org.postgresql.Driver"</property>
		<property name="URL">"jdbc:postgresql://localhost:5432/iap_db"</property>
		<property name="user">"postgres"</property>
		<property name="password">"postgres"</property>
	</component>
	
3,运行
        右击:/s2jdbc-tutorial/s2jdbc-gen-build.xml
        选择运行方式:ANT构建
        
4,生成的代码在src下
