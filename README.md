Documentation: http://rll.berkeley.edu/trajopt

Work with PCL 1.8, VTK 8.0, OSG 3.4 on Ubuntu 16.04

- install openrave
  - https://scaron.info/teaching/installing-openrave-on-ubuntu-16.04.html
  - http://fsuarez6.github.io/blog/workstation-setup-xenial/

- install Gurobi
    - Download current version gurobi*** into your ~/Downloads folder. <br>
    ` cd ~/Downloads `<br> 
    ` tar xvfz gurobi***_linux64.tar.gz` <br> 
    ` sudo mv gurobi*** /opt/ `<br> 
    - Getting a license <br>
    - go to http://www.gurobi.com/downloads/licenses/license-center and requrest an university lisence. Once you have a free university lisence, <br>
    `cd /opt/gurobi***/linux64/bin` <br>
    `./grbgetkey <LICENSE NUMBER GOES HERE>` <br>
    - Set GUROBI_HOME environment variable. <br>
    `echo export GUROBI_HOME="/opt/gurobi***/linux64" >> ~/.bashrc` <br>

- install trajopt  
mkdir build && cd build <br>
cmake .. -DOSG_DIR=/usr/local/lib64/ <br>
make -j
  - add /path/to/trajopt:/path/to/build_trajopt/lib:/usr/local/lib:/usr/local/lib64 to PYTHONPATH
