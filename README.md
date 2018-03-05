# README #

## Installation ##

Run `install.py` to setup a password.

### Dependencies ###

Install all necessary python packages, `srecord` for `srec_cat`, and `texlive` for `pdflatex`.

## Configuration File ##

Each folder name in `firmware/` corresponds to an available `version`.

## Examples ##

Input example:

~~~~
>>type config\0000.cfg
[DEFAULT]
house_id = 0000
tsch = 2_and_1_shared_schedule
total_gateways = 4
total_environmental = 4
total_wearables = 4
~~~~

Output example:

~~~~
>>python run.py 0000
No explicit system version specified. Using default system version: dangermouse.42
Password:
SPHERE Report
--------------------------------------------
House ID: 0000
Network ID: 121
Date: 20171025
Total Gateways: 4
[Device: 001] Image created. Root Gateway (F): 00124b0000007901
[Device: 064] Image created. Root Gateway (G): 00124b0000007940
[Device: 002] Image created. Gateway (F): 00124b0000007902
[Device: 065] Image created. Gateway (G): 00124b0000007941
[Device: 003] Image created. Gateway (F): 00124b0000007903
[Device: 066] Image created. Gateway (G): 00124b0000007942
[Device: 004] Image created. Gateway (F): 00124b0000007904
[Device: 067] Image created. Gateway (G): 00124b0000007943
Total Environmental: 4
[Device: 128] Image created. Environmental: 00124b0000007980
[Device: 128] Image created. Water sensor: 00124b0000007980
[Device: 129] Image created. Environmental: 00124b0000007981
[Device: 129] Image created. Water sensor: 00124b0000007981
[Device: 130] Image created. Environmental: 00124b0000007982
[Device: 130] Image created. Water sensor: 00124b0000007982
[Device: 131] Image created. Environmental: 00124b0000007983
[Device: 131] Image created. Water sensor: 00124b0000007983
Total Wearables: 4
[Device: 192] Image created. Wearable: a0e6f80079c0
[Device: 193] Image created. Wearable: a0e6f80079c1
[Device: 194] Image created. Wearable: a0e6f80079c2
[Device: 195] Image created. Wearable: a0e6f80079c3
Creating labels..
Labels written in labels.pdf
~~~~
