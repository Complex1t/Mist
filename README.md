# Mist

Mist is a Spigot Development Library focused on getting large-scale Spigot plugins up and running. It's mainly useful in easily making big plugins since it already provides a lot of the functionality and the developer just has to implement it. There are ideas for a lite version that just contains boilerplate code for smaller plugins and also a full game mode API.

## Notes

Mist is built using Kotlin meaning the size of the plugin is bloated by about 800kb. This doesn't affect performance whatsoever it just increases the jar size. *This will NOT halt performance at all.*. This is because the standard Kotlin library has to be shaded into the jar. It is not shaded in the Mist jar so must be in your project by providing this dependency along with the maven-shade-plugin
```xml
<dependency>
    <groupId>org.jetbrains.kotlin</groupId>
    <artifactId>kotlin-stdlib-jdk8</artifactId>
    <version>${kotlin.version}</version>
    <scope>provided</scope>
</dependency>
```

## Installation
To use this project simply add the following dependency from jitpack, replacing VERSION with the current version
```xml
<dependency>
    <groupId>com.github.Relaxing9</groupId>
	<artifactId>Mist</artifactId>
	<version>VERSION</version>
</dependency>
```

## License
[MIT](https://choosealicense.com/licenses/mit/)