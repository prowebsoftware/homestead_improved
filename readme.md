# Laravel Homestead: Improved

An improved version of Laravel Homestead.

The improvements made so far:

 - port 5000 is automatically forwarded to accommodate Heroku's Foreman
 - SSH keys setup completely removed. Just `vagrant up` and `vagrant ssh`.
 - global composer auto-updates
 - apt-get update is autoexecuted
 - folders are mapped by default as "current" to "Code". This means you don't have to change folder mapping if you're always using the root folder of the project as the mapping. The folder the Vagrantfile is in will be mapped to the `/home/vagrant/Code` folder in the VM.

 PRs for further improvements welcome.

 ## Todo

  - open remote connections to MySQL and PostgreSQL, removing need to forward ports like 33060 to 3306
  - open port 80 for ease of access via, e.g., `homestead.app` rather than `homestead.app:8000` as it is now
  - ...?