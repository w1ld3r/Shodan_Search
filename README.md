# Shodan Search

Information gathering on IP adress or Hostname with Shodan.

Gather:

* IP Adress
* City
* Country Name
* Organization
* ISP
* Last Update
* Open Ports
* Domain Name
* Honey Score
* Vulnerabilities
* GPS coordinates

With [Folium](https://python-visualization.github.io/folium/quickstart.html#Markers), it creates an HTML map to locate the server. 

## Getting Started

### Prerequisites

Install python3 and pip:
```bash
sudo apt install python3 python3-pip
```

### Installing

The installation has been tested in Debian bullseye/sid x86\_64 (february 2019)

#### Clone the project
```bash
git clone https://github.com/x1n5h3n/Shodan_Search.git
```

#### Move in the project folder
```bash
cd Shodan_Search
```

#### Install the necessary Python packages:
```bash
pip3 install -r requirements.txt
```

#### Add your Shodan API key
Replace `your_shodan_api_key`  with your Shodan API Key .
```bash
sed -i -e 's/XXXXX/your_shodan_api_key/g' shodan_search.py
```

### Usage

Gather informations on IP address:
```bash
python3 shodan_search.py -t 8.8.8.8
```

Gather informations on Hostname:
```bash
python3 shodan_search.py -t google.com
```

Print help:
```bash
python3 shodan_search.py -h
```

## Authors

* **[x1n5h3n](https://github.com/x1n5h3n)**

## License

This project is licensed under the GPLv3 License - see the [LICENSE](LICENSE) file for details.
