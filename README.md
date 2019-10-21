
# mqsql-xml-sdk



**Steps to Use:**

1) Clone this repo to your local and make chages to the DB configuration as per your ennvironment. (Create Config files to pass in the DB properties )

2) Publish this connector your your exchange.

3) In the API in which you want to use this connector, download the connector into pallette, and add below code to the pom.xml:
```<build>
		<plugins>
			<plugin>
				<groupId>org.mule.tools.maven</groupId>
				<artifactId>mule-maven-plugin</artifactId>
				<version>${mule.maven.plugin.version}</version>
				<extensions>true</extensions>
				<configuration>
				<sharedLibraries>
                     <sharedLibrary>
                            <groupId>mysql</groupId>
                            <artifactId>mysql-connector-java</artifactId>
                        </sharedLibrary>
                    </sharedLibraries>
				</configuration>
			</plugin>
		</plugins>
		 
	</build>```


