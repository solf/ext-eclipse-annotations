# ext-eclipse-annotations
External annotations for null-analysis in Eclipse.

This is a collection that I've assembled over the years of using Eclipse's
null-analysis external annotations facility.

For JDK 1.8 (Oracle's) I've used annotations under jdk/1.8/rt.jar/

For later JDKs (particularly 11, OpenJDK and Amazon's) I'm using annotations
under jdk/any/all.jar/

For all the Maven dependencies used in projects I'm using annotations under
maven/

To use external annotations with Maven under Eclipse you'll need something like
https://github.com/lastnpe/eclipse-external-annotations-m2e-plugin

Personally I'm using a modified version that let's me set Maven external 
annotation path in eclipse.ini:
-Dm2e.eea.annotationpath.maven=/ext-eclipse-annotations/maven

See https://github.com/lastnpe/eclipse-external-annotations-m2e-plugin/issues/24
for some discussions about this.
