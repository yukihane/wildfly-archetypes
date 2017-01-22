Original `README.md` is `README.orig.md` .

# What' this

Updated pom.xml for WildFly10.1.x .


# Install

    /bin/bash generate-blank.sh -a

for generating blank archetypes.
Then,

    cd [archetype-directory]
    mvn clean install
    mvn archetype:update-local-catalog

Following archetypes are will work fine,
- wildfly-javaee7-webapp-archetype
- wildfly-javaee7-webapp-blank-archetype
- wildfly-javaee7-webapp-ear-archetype
- wildfly-javaee7-webapp-ear-blank-archetype

but others may not work correctly.

# Usage

    mvn archetype:generate \
    -DarchetypeGroupId=com.github.yukihane.wildfly.archetype \
    -DarchetypeArtifactId=wildfly-javaee7-webapp-archetype \
    -DarchetypeCatalog=local

etc.
