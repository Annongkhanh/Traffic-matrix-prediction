# Traffic-matrix-prediction

SDN traffic matrix prediction with LSTM

2 networks: Géant(2001) and Zamren

Géant network dataset dowloaded from: https://totem.info.ucl.ac.be/dataset.html

Zamren network dataset generated from SDN emulated by mininet and POX controller using tcpreplay, running in an Ubuntu 21.04 virtual machine.

To install mininet, please read installation guide from http://mininet.org/download/, option 2: Native Installation from Source.

To install POX controller, running this command in terminal:

    git clone http://github.com/noxrepo/pox

Jupyter Notebook files was created and running in Google Colab (https://colab.research.google.com/).

To simulate these network, clone this git to POX folder:

We run POX controller using this command:

    python2 pox.py openflow.spanning_tree --no-flood --hold-down openflow.discovery basic_forwarding traffic_observation  

If you want to change the interval (default = 30 seconds) and save the measured traffic matrixes in a file, change the value of interval and add the path to the output in traffic_observation.py

We run mininet simulation of Zamren topology by this command:

    sudo python2 Zamren








