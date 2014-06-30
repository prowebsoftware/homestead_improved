# Laravel Homestead: Improved

An improved version of Laravel Homestead.

The improvements made so far:

 - port 5000 is automatically forwarded to accommodate Heroku's Foreman
 - SSH keys setup completely removed. Just `vagrant up` and `vagrant ssh`.

 PRs for further improvements welcome.

 ## Todo

  - open remote connections to MySQL and PostgreSQL, removing need to forward ports like 33060 to 3306
  - open port 80 for ease of access via, e.g., `homestead.app` rather than `homestead.app:8000` as it is now
  - autoexecute `sudo apt-get update`
  - ...?