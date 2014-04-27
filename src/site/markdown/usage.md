## Introduction
Doxia is a content generation framework. A [Doxia module][doxiamodule] is an implementation of a given markup language like APT, Docbook, or Markdown.

Markdown is an elegant markup language.

This doxia modules parses files in the Markdown syntax.

## Use for Maven site

You can use Markdown instead of ATP in the <code>mvn site goal</code>.

## Write Markdown files
Write the Markdown files in <code>src/site/markdown</code>

## Edit your POM
Edit your POM to reference the module in the <code>maven-site-plugin</code>


    <build>    
        <plugins>    
           <plugin>    
             <groupId>org.apache.maven.plugins</groupId>
             <artifactId>maven-project-info-reports-plugin</artifactId>
             <version>2.7</version>
           </plugin>
           <plugin>
             <groupId>org.apache.maven.plugins</groupId>
             <artifactId>maven-site-plugin</artifactId>
             <version>3.3</version>
             <dependencies>
               <dependency>
                 <groupId>org.apache.maven.doxia</groupId>
                 <artifactId>doxia-module-markdown</artifactId>
                 <version>1.5</version>
               </dependency>
             </dependencies>
             <configuration>
               <inputEncoding>UTF-8</inputEncoding>
               <outputEncoding>UTF-8</outputEncoding>
             </configuration>
           </plugin>
         <!-- other  plugins ... ->
         </plugins>
    <!-- other build instructions -->
    </build>


## Use in Java code

You can also [use the Doxia framework in your Java program](http://maven.apache.org/doxia/modules/index.html#Using_A_Doxia_Module).

[doxiamodule]: http://maven.apache.org/doxia/modules/index.html
