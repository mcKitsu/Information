
# 如何使用mcKitsu私有Maven倉庫
### 1.建立Github Token

進入[Github Token](https://github.com/settings/tokens/new)建立專用Token

Select scopes請勾選**repo**、**write:packages**、**read:packages**

### 2.新增maven設定檔

預設maven資料夾路徑為C:\\Users\\**USER_NAME**\\.m2

在maven目錄下新增檔案**settings.xml**並複製以下文字

將**YOUR_NAME**改成Github name

將**YOUR_TOKEN**改為步驟1所建立的**Token**

```a
<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0
                      http://maven.apache.org/xsd/settings-1.0.0.xsd">

  <activeProfiles>
    <activeProfile>github</activeProfile>
  </activeProfiles>

  <profiles>
    <profile>
      <id>github</id>
      <repositories>
        <repository>
          <id>central</id>
          <url>https://repo1.maven.org/maven2</url>
          <releases><enabled>true</enabled></releases>
          <snapshots><enabled>true</enabled></snapshots>
        </repository>
        <repository>
          <id>github</id>
          <name>GitHub mcKitsu Apache Maven Packages</name>
          <url>https://maven.pkg.github.com/mcKitsu</url>
        </repository>
      </repositories>
    </profile>
  </profiles>

  <servers>
    <server>
      <id>github</id>
      <username>YOUR_NAME</username>
      <password>YOUR_TOKEN</password>
    </server>
  </servers>
</settings>
```

### 3.使用mcKitsu私有遠端倉庫

於專案pom.xml內新增以下碼

```
<repositories>
    <repository>
        <id>github</id>
        <url>https://maven.pkg.github.com/mcKitsu</url>
    </repository>
</repositories>
```

### 4.Enjoy
