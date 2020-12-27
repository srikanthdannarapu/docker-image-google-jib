# spring boot docker image with google-jib-example

go to C:\Users\sreekanth\.m2 path and add below docker credentials in settings.xml file

<servers>
    <server>
        <id>registry.hub.docker.com</id>
        <username><DockerHub Username></username>
        <password><DockerHub Password></password>
    </server>
</servers>


mvn clean compile jib:build

docker run -it -p 8080:8080 sdannarapu/google-jib-image-example