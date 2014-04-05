mvn-repo
========

mvn-repo
========

To use this Maven repository, add the following profile to your settings.xml:

```
<profile>
	<id>infernozeus</id>
	<repositories>
		<repository>
			<id>mvn-repo</id>
			<url>https://raw.github.com/InfernoZeus/mvn-repo/master/releases</url>
			<snapshots>
				<enabled>false</enabled>
			</snapshots>
		</repository>
		<repository>
			<id>mvn-repo-snapshot</id>
			<url>https://raw.github.com/InfernoZeus/mvn-repo/master/snapshots</url>
			<snapshots>
				<enabled>true</enabled>
				<updatePolicy>always</updatePolicy>
			</snapshots>
			<releases>
				<enabled>false</enabled>
			</releases>
		</repository>
	</repositories>
</profile>
```

And then activate it:

```
<activeProfiles>
	<activeProfile>infernozeus</activeProfile>
</activeProfiles>
```
