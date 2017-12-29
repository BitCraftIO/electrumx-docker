# electrumx-docker
Dockerfile for [BitCraft's ElectrumX](https://github.com/BitCraftIO/electrumx) on Ubuntu with leveldb and daemontools.

## Usage
### Step 1. Configuration
```
git clone https://github.com/BitCraftIO/electrumx-docker.git
cd electrumx-docker
```

Then,Edit `env/COIN` to your coin.

Edit `env/DAEMON_URL` accordingly.Need to match your daemon.

For AltCoins,edit your coin class in `env/coins.py`.`env/coins.py` will be append to [electrumx/lib/coins.py](https://github.com/kyuupichan/electrumx/blob/master/lib/coins.py)

Leave others defaults

### Step 2.Run
Build your docker image:
```shell
      docker build -t electrumx .
      docker run -v -idt electrumx
```

## THANKS

### Warmly welcome all kinds of suggestions

Thanks for suggestions from:

[kyuupichan](https://github.com/kyuupichan/electrumx)

[qinshulei](https://github.com/qinshulei)

