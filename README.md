Spring Boot Test app:
https://github.com/spring-projects/spring-petclinic

Run this to build it:
mvn install

Download visualvm:
https://visualvm.github.io/download.html

Download Azul JDK 11:
https://www.azul.com/downloads/?package=jdk#download-openjdk

Download jHiccup:
https://www.azul.com/products/components/jhiccup/

Download and build HdrHistogramAnalyzer:
https://github.com/HdrHistogram/HdrHistogram
Run this to build it:
mvn install

Download GCLogAnalyzer:
https://docs.azul.com/prime/GC-Log-Analyzer

Download Apache Jmeter:
https://jmeter.apache.org/download_jmeter.cgi

CLI snippets:
java -jar GCLogAnalyzer2.jar &
./visualvm &
./jmeter &
java -jar target/HistogramLogAnalyzer-1.0.4-SNAPSHOT.jar
java -Xmx64m '-Xlog:gc*=debug:file=test_zulu_18.log'  -javaagent:../jHiccup-2.0.10/jHiccup.jar -jar target/spring-petclinic-2.7.0-SNAPSHOT.jar
