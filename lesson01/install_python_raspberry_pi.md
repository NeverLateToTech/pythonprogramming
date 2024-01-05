* Check current Python version

  > python --version

* Download python dist tar ball (ex: for version 3.12)

  > wget https://www.python.org/ftp/python/3.12.1/Python-3.12.1.tgz

* Update os packages

  > sudo apt-get update

* Install additional packages

  > sudo apt-get install build-essential tk-dev libncurses5-dev libncursesw5-dev libreadline6-dev libdb5.3-dev libgdbm-dev libsqlite3-dev libssl-dev libbz2-dev libexpat1-dev liblzma-dev zlib1g-dev libffi-dev

* Extract downloaded Python tar ball

  > tar -xvf Python-3.12.1.tgz

* Execute configure script

  > cd Python-3.12.1
  > 
  > ./configure --enable-optimizations  

* Execute make command

  > make -j 4
  > 
  > sudo make altinstall

* Verify new python distribution

  > python3.12 --version
  
* Change default system verion

  > python --version
  >
  > ls /usr/bin/python* -latr | grep -v config
  >
  > whereis python3.12
  >
  > sudo rm /usr/bin/python3
  >
  > sudo ln -s /usr/local/bin/python3.12 /usr/bin/python3
