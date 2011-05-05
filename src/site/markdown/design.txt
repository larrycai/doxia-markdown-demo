## Maven
The code is a Maven project.

## Doxia Module

The code is a [doxia module](http://maven.apache.org/doxia/developers/index.html#Create_a_New_Doxia_Module).

 * The package is <code>org.apache.maven.doxia.module.markdown</code>
 * The Parser is <code>MarkdownParser</code>. This parser simply invokes the Markdownj parser.
 * A <code>MarkdownParseException</code> can only be raised when opening the input file raises an IOException
 * The <code>MarkdownSiteModule</code> defines that the markdown resources are in {{src/site/markdown}} and have extension .txt
 * The <code>MarkdownSink</code> is an empty implentation of <code>AbstractTextSink</code>
 * The <code>MarkdownSinkFactory</code> builds a <code>MarkdownSink</code>
 
## Markdownj parser
This module is based on the [Markdownj](http://maven.apache.org/doxia/developers/index.html#Create_a_New_Doxia_Module) parser by [Alex Coles](http://maven.apache.org/doxia/developers/index.html#Create_a_New_Doxia_Module).