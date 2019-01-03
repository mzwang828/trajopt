Documentation: http://rll.berkeley.edu/trajopt

Work with PCL 1.8, VTK 8.0, OSG 3.4 on Ubuntu 16.04

- install openrave
    https://scaron.info/teaching/installing-openrave-on-ubuntu-16.04.html
    http://fsuarez6.github.io/blog/workstation-setup-xenial/

- install Gurobi

    Download current version gurobi*** into your ~/Downloads folder.
    cd ~/Downloads
    tar xvfz gurobi***_linux64.tar.gz
    sudo mv gurobi*** /opt/
    Getting a license
    go to http://www.gurobi.com/downloads/licenses/license-center and requrest an university lisence. Once you have a free university lisence,
    cd /opt/gurobi***/linux64/bin
    ./grbgetkey <LICENSE NUMBER GOES HERE>
    Set GUROBI_HOME environment variable.
    echo export GUROBI_HOME="/opt/gurobi***/linux64" >> ~/.bashrc

mkdir build && cd build
cmake .. -DOSG_DIR=/usr/local/lib64/
make -j
