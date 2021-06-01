# This is a community effort to draw the nimbus logo on beaconcha.in's graffitiwall. 

## get started
clone repo with `git clone https://github.com/tennisbowling/graffitiwall-nimbus`, then enter the directory with `cd graffitiwall-nimbus` \
install requirements with `python3 -m pip install -r requirements.txt` \
## nimbus
run nimbus with rpc enabled, just add `--rpc` to the nimbus process \
run the drawer with `python3 Drawer.py --network mainnet --settings-file settings.ini --client nimbus` \
## prysm
on the validator instance, not the beacon node, add `--graffiti-file $HOME/graffiti.txt` \
run the drawer with `python3 Drawer.py --network mainnet --settings-file settings.ini --client prysm --out-file $HOME/graffiti.txt` \
## lighthouse
on the validator instance, not the beacon node, add `--graffiti-file=$HOME/graffiti.txt` \
run the drawer with `python3 Drawer.py --network mainnet --settings-file settings.ini --client lighthouse --out-file $HOME/graffiti.txt` \
## teku
on the validator instance, not the beacon node, add `--validators-graffiti-file=$HOME/graffiti.txt` \
run the drawer with `python3 Drawer.py --network mainnet --settings-file settings.ini --client teku --out-file $HOME/graffiti.txt` \

you are contributing to the graffitiwall next time you propose a block! \
thanks to stake-house for making the original \
https://github.com/stake-house/DecentralizedGraffitiDrawing
