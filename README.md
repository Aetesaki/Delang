# Delang
A set of scripts for the constructed language Delang and its Illomi 
culture

## Getting Started

These instructions will get you a copy of the project up and running on 
your local machine for your entertainment or curiousity.

### Prerequisites

To use these scripts you need to have a fuctioning bash environment AND 
a git cloner on your system, preferably you should have a running linux 
system as neither MacOS or Windows have both bash and git installed as 
default.

#### Installing Linux on Windows
* Click the start button, and select settings
* Search for and run "Turn Windows Features On Or Off"
* In the window, search for and  enable “Windows Subsystem for Linux”
* Restart the computer
* After restart, open Windows Store
* Search for Linux
* Open one of the avaiable Linux distros (make sure you actually open an
 actual Linux distro, as not all search result are valid)
* Install your preferred Linux distro
* When the Linux distro has been installed, open it and follow the 
onscreen setup instructions

### Installing
To download these scripts open a terminal, of if you are using Windows, 
open the previously installed Linux distro

* mkdir git
* cd git
* git clone https://github.com/Aetesaki/Delang.git

To make the scripts available use this command
* echo "$HOME/git/Delang:$PATH" >> .bashrc

At this point you should close your terminal, and reopen it to use the 
scripts

### Keeping the scripts up to date
To keep the scripts up to date with the git repository, you should 
periodically pull the repository. If you use these scripts seldom, 
please do that before running any of the scripts.

Open a terminal, or if you are using Windows, open the previously 
installed Linux distro
* cd git/Delang && git pull | cd

## How to use the scripts
To use the scripts, open a terminal, or if you are using Windows, open 
the previously installed Linux distro, and type the name of the script, 
and the script will give you a short description on how to use it. 

For more information, you can use the --help option available in all 
scripts. 

For version information, use the --version option.

## Scripts
### Converters
#### Blood pressure converters
* mmhg2lunu – Convert mmHg to lunu
* lunu2mmhg – Convert lunu to mmHg

##### Note
Normal blood pressure in lunu, 0/0, is a blood pressure within the range
of 110-125/75-85 mmHg. Any number within that range will be converted to
0/0 lunu. On the flip side, 0/0 lunu will be converted to normal/normal.

Any hypertension is converted to positive numbers in lunu, while any
hypotension is converted to negative numbers in lunu.

1 lunu = 4 millimeter = 0.16 inches

#### Temperature converters
* degc2peu – Convert degree celcius to peu
* peu2degc – Convert peu to degree celcius

##### Fahrenheit support
To convert from fahrenheit to peu, clone RandomScripts using the 
following commands:
* cd ~/git
* git clone https://github.com/Aetesaki/RandomScripts.git
* echo "$HOME/git/RandomScripts:$PATH" >> .bashrc

Close your terminal, and reopen it. Now you will be able to convert
fahrenheit to peu and back again using the following commands:
* degf2degc 100 | degc2peu – Converts 100°F to 15.82 peu
* peu2degc 15.82 | degc2degf – Converts 15.82 peu to 99.99°F

This method is called piping, and is common in Linux

##### Common temperatures in peu
* Water freezing: 0°C = 32°F = -14.4 peu
* Body temperature of a human: 37°C = 98.6°F = 15.2 peu
* Water boiling at sea level: 100°C = 212°F = 65.6 peu
* -40°: -40°C = -40°F = -46.4 peu
* Absolute zero: -273.15°C = -459.67°F = -232.92 peu

