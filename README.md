<html>
<body>


Here you can find information on the current status of Tahopens's "mavenization" effort. Please make sure to follow the standards and guidelines when converting projects so that we can keep our codebase as consistent as possible.
The Parent Poms

The parent poms will do a great deal of the leg-work to accomplish the basics of your build. When choosing a parent pom version, please consult the latest release tag at https://github.com/tahopen/maven-parent-poms

The structure of the parent poms is this:

       tahopen-parent-pom

               |

     tahopen-ce-parent-pom

               |
   tahopen-ce-jar-parent-pom

               |

  tahopen-ce-bundle-parent-pom


## tahopen-parent-pom

This pom is not meant to be used directly. It contains much of what may be needed in both the Community Edition (ce) stacks of parent poms.
tahopen-ce-parent-pom

``` xml
<parent>
  <groupId>org.tahopen</groupId>
  <artifactId>tahopen-ce-parent-pom</artifactId>
  <version>0.1.0-SNAPSHOT</version>
</parent>


Used primarily for ce assemblies
tahopen-ce-jar-parent-pom

``` xml
<parent>
  <groupId>org.tahopen</groupId>
  <artifactId>tahopen-ce-jar-parent-pom</artifactId>
  <version>0.1.0.0-SNAPSHOT</version>
</parent>


Used primarily for ce jar artifacts and bundles without Javascript
tahopen-ce-bundle-parent-pom


``` xml
<parent>
  <groupId>org.tahopen</groupId>
  <artifactId>tahopen-ce-bundle-parent-pom</artifactId>
  <version>0.1.0.0-SNAPSHOT</version>
</parent>


Used primarily for ce bundles that contain Javascript


</body>
</html>
