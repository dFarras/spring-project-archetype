# Purpose

<p>This archetype allows you to create a basic spring application to be able to create it and start working as fast as 
possible. I am aware that some of its defined dependencies might not be suitable for everyone, but this is for personal 
use.
<br>Although it is for personal use it will be improved and if anyone wants to request a change you can do so at this 
project board.<br> Add link here <br>

> Those requests will be answered as fast as possible, but I might decide not to implement them if they 
are not suitable for my purposes. In that case you can just create a fork.


# Usage

<p>Since it is just a simple archetype you just have to do the same as in any other archetype. But in case someone needs
some guidance I leave here the way to use it:</p>

>Clone this project: <i>git clone add-url</i>

>Install in your local maven installation: <i>mvn install</i>

>Create a repo: (use this command in one line, or separate every line with a backslash)
>><i>mvn archetype:generate <br>
> -DarchetypeArtifactId=org.dfarras <br>
> -DarchetypeGroupId=spring-project-archetype <br>
> -DarchetypeVersion=1.0 <br>
> -DgroupId=[your.project.group.id] <br>
> -DartifactId=[your-project-artifact-id] <br>
> -Dversion=[your-project-version]</i>

<p>When using this archetype be careful since groupId content is used to create the repository file structure. 
A file will be created by every word between dots in that groupId.</p>  

# Archetype
<p>Although I am offering this way to create a fast spring project I want to left here a way for anyone to create his or her own archetypes.</p>

## Create archetype from scratch
<p>You will see that it is quite similar to the command above since the main difference is that -B parameter, apart from a couple of parameters. Just use this command:</p>

>mvn archetype:generate -B -DarchetypeArtifactId=maven-archetype-archetype \
>-DarchetypeGroupId=maven-archetype \
>-DgroupId=[your.archetype.group.id] \
>-DartifactId=[your.archetype.artifact.id]

## Create from another project
<p>Right in your project folder use this simple command:</p>

> mvn archetype:create-from-project

<p>To find the newly created project only go to: <i>project > target > generated-sources</i></p>

# External sources
Of course this has not been done all alone, here you have the links used to create this project (hope they help you too):
<ul>
    <li><a href="https://maven.apache.org/guides/introduction/introduction-to-archetypes.html">Maven official documentation</a></li>
    <li><a href="https://www.baeldung.com/maven-archetype">Baeldung archetype page</a></li>
</ul>