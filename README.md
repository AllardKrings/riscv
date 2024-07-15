#Argo Workflow Template

This template can be used on riscv64-architecture to clone a git-repo and execute Maven on the cloned source. 

#pom.xml

The POM that is used by Maven compiles the java-code, creates a WAR-file, builds an OpenLiberty image containing the WAR-file and pushes the image to Docker Hub.
The exec-maven-plugin is used fro building and pushing the image. It uses docker mounted from the host.
