# Scala-cli version-specific cross publish example

1. publish the library for both versions
```
scala-cli publish local cross-lib --organization com.example --version 0.0.1 -S 3
```
```
scala-cli publish local cross-lib --organization com.example --version 0.0.1 -S 2.13
```

2. run the app with both versions
```
scala-cli cross-app/Example.scala -S 3
//uses V3
```
```
scala-cli cross-app/Example.scala -S 2.13
//uses V2
```