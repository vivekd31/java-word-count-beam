# java-word-count-beam
* In 44-517 folder opened the powershell as administrator and then by using the following commands generated the maven project <br>
```PS> mvn archetype:generate `
 -D archetypeGroupId=org.apache.beam `
 -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
 -D archetypeVersion=2.36.0 `
 -D groupId=org.example `
 -D artifactId=word-count-beam `
 -D version="0.1" `
 -D package=org.apache.beam.examples `
 -D interactiveMode=false ```
* Added the sample.txt file in the folder and copied content of shakespeare's sonnets.
* Run the wordcount beam using following maven command 
 ```
 PS> mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
    -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner
  ```

![image](https://github.com/vivekd31/java-word-count-beam/blob/master/Output.png)
