# The Humble Roots Project
**Home Automation Applied To Medical Cannabis Cultivation**

The Humble Roots Project is a grow room automation system designed to meet indoor horticulture
challenges using open software, open hardware and readily available consumer appliances. The project
blends these elements together into an inexpensive, reliable, efficient, automated system, with a focus
on sustainability.

The application of the concepts and technology used as part of the Humble Roots Project is not limited
to indoor growing or horticulture; it has far-reaching applications to many other automation scenarios
where sensors, actuators, rules and data visualization are combined to solve a problem. 

For more details, refer to the [project documentation](./docs/HumbleRootsProject.pdf).

![Humble Roots Lab](./docs/lab.png "Humble Roots Lab")

## Required Arduino Dependencies



## Required Python Dependencies

### [Install the Mosquitto MQTT broker](http://mosquitto.org/)

```
sudo apt-get install mosquitto
```

### [Install the Python MQTT client](https://www.eclipse.org/paho/clients/python/)

```
git clone http://git.eclipse.org/gitroot/paho/org.eclipse.paho.mqtt.python.git
cd org*
sudo python setup.py install
```

### [Install the PySerial package](https://pypi.python.org/pypi/pyserial)

```
wget https://pypi.python.org/packages/source/p/pyserial/pyserial-2.7.tar.gz#md5=794506184df83ef2290de0d18803dd11
gunzip pyserial-2.7.tar.gz
tar xvf pyserial-2.7.tar
cd  pyserial-2.7
sudo python setup.py install
```

### [Install the Hashids package](http://hashids.org/python/)

```
git clone https://github.com/davidaurelio/hashids-python.git
cd hashids-python
sudo python setup.py install
```

## Optional Python Dependencies

The following packages only need to be installed if used in the project.

The PushBullet API uses TLS and validates server certificates.
Depending on your OS or your distribution, some dependencies may not be present by default and need to be added for PushBullet to build and work properly.

### Install the Python development tools

```
sudo apt-get install python-dev
```

### Install Python pip

```
sudo apt-get install python-pip
```

### Install libffi-dev needed to build PyOpenSSL

```
sudo apt-get install libffi-dev
```

### Install and build PyOpenSSL and its dependencies

```
sudo pip install pyopenssl ndg-httpsclient pyasn1
```

### [Install the PushBullet Python client](https://github.com/Azelphur/pyPushBullet)

```
git clone https://github.com/Azelphur/pyPushBullet.git
cd pyPushBullet
sudo python setup.py install
```

### [Install InfluxDB](http://influxdb.com/)

InfluxDB is the time-series database used by the project to store sensor data.

For installing InfluxDB on the Raspberry Pi, or another ARM system, see [here](http://www.pihomeserver.fr/en/2014/11/29/raspberry-pi-home-server-installer-influxdb/)

### [Install Grafana](http://grafana.org/)

Grafana produces beautiful charts and works with InfluxDB.

