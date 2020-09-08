
# 如何將Repository發布為Packages

執行此步驟時請先執行[如何使用mcKitsu私有Maven倉庫](./repo.md)

### 1.於Maven專案內編輯pom.xml

新增以下內碼，並將**YOUR_REPO_NAME**替換為在Github上的專案名稱

假設為專案[KitsuLib](https://github.com/mcKitsu/KitsuLib)，就將**YOUR_REPO_NAME**改為**KitsuLib**

```
<distributionManagement>  
	 <repository> <id>github</id>  
		 <name>GitHub mcKitsu Apache Maven Packages</name>  
		 <url>https://maven.pkg.github.com/mcKitsu/YOUR_REPO_NAME</url>  
	 </repository>
</distributionManagement>
 ```


### 2.上傳包至Github

於專案內執行 **mvn reploy**

### 3.Enjoy
