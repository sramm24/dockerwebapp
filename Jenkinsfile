node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub_cred') {

        def customImage = docker.build("sramm24/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
