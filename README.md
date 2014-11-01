# Vagrant Docker VM
-------------------

If you are running Docker on a Mac or Windows then you need a linux VM to run your Docker containers on.  Docker offers a tool called boot2docker which basically is a simple VM manager that can be used to init a new VM to be used by Docker as you start to create/build images and need to run the containers.

That said, boot2docker does have some limitations, such as it is hare (not impossible) to mount your host file system to your VM so your Docker containers has access to them, very useful if you are using Docker to to development on a project.  Because of this limitation a preferred way to use Docker on Mac and Windows is to use Vagrant to create/provision a VM to be used by Docker, which gives you a little more flexiblity on defining what is on taht VM, such as mounting file systems etc.  This sample project just provides a Vagrantfile and instructions on how to use Vagrant to create and associate to Docker instead of using boot2docker.

`NOTE` - As of [Docker 1.3](https://blog.docker.com/2014/10/docker-1-3-signed-images-process-injection-security-options-mac-shared-directories/) it now sounds like it is much easier to mount file systems.  However you still might want to use Vagrant if you are more use to it or are using a combination of both Docker and Vagrant (Puppet/Chef) VMs.

## Setup

Start by cloning this profile;