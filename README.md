Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).



Manual steps for installation of java
----------------------------------------------------
* for jdk13

```
   https://java.tutorials24x7.com/blog/how-to-install-openjdk-13-on-ubuntu
   sudo mkdir /usr/java
   cd /usr/java/
   wget https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
   sudo tar -xvzf openjdk-13.0.2_linux-x64_bin.tar.gz
   sudo nano /etc/profile
   sudo update-alternatives --install "/usr/bin/java" "java" "/usr/java/jdk-13.0.2/bin/java" 1
   sudo update-alternatives --install "/usr/bin/javac" "javac" "/usr/java/jdk-13.0.2/bin/javac" 1
  java --version
```

* for java 11 and 17
--------------------

```
sudo apt update
sudo apt install openjdk-11-jdk -y
sudo apt install openjdk-17-jdk -y
```
