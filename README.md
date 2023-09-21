# DashHourApp

Dashboard Dash application which displays current time (curl from https://quelleheureestil.fr) and a graph of the time series every 5 minutes using cron. There is also a daily report updating each day at 8pm. The server is hosted on a AWS Linux virtual machine.

## Production

- AWS URL: http://16.170.37.227/ or http://ec2-16-170-37-227.eu-north-1.compute.amazonaws.com (currently down, you can host it yourself)

## Usage


* Clone this repository, from your local machine:
  ```bash
  git clone https://github.com/LynaMOSTEFACHAA/Python-Git-Linux-IF4.git
  ```
* Get the requirements
  ```bash
  # Install requirements with pip
  pip install -r requirements.txt
  #or just pip install every import e.g. dash:
  pip install dash
  ```

* Start the application
  ```bash
  $ crontab -e
  $ */5 * * * * python3 your/path/to/dashboardUpdated.py
  ```
  or
    ```bash
  $ crontab -e
  $ */5 * * * * bash your/path/to/run_dash.sh
  ```

* Important: If you use it locally, do not forget to adapt all paths in the script run_dash and the application dashboardUpdated.

## Author

- Nassim AILALI: nassim.ailali@edu.ece.fr
- Lyna MOSTEFA CHAA: lyna.mostefa_chaa@edu.devinci.fr

## 📚​ Documentation

Dash: https://dash.plotly.com

Python libraries: https://docs.python.org/fr/3/library/
