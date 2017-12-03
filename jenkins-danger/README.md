# jenkins-danger
Sample of jenkins + danger. See also [jenkins-danger-sample-project]().

## prerequiste
- Set your github API token to an environment variable.

```
export DANGER_GITHUB_API_TOKEN=YOUR_GITHUB_API_TOKEN_HERE
```

## usage

```sh
$ ./build #build docker image
$ ./run #run the image in a container
```

And then, Jenkins server is available at `http://localhost:8080`.
Jenkins requires an initial admin password generated when the process activated.

You can get the password by login to the container:

```sh
$ ./shell #login shell of the container
$ cat /var/jenkins_home/secrets/initialAdminPassword
```