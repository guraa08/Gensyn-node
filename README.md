# Gensyn-node

GPU Mode

Install Sudo
````
apt update && apt install -y sudo
`````

Install dependencies
```
sudo apt update && sudo apt install -qy net-tools python3 python3-venv python3-pip curl wget screen git lsof iproute2 nano unzip build-essential
```

Install Node.js and NPM
```
curl -sSL https://raw.githubusercontent.com/zunxbt/installation/main/node.sh | bash
```

Clone Rl-Swarm
```
git clone https://github.com/gensyn-ai/rl-swarm
cd rl-swarm
```

Setup Config
```
cd $HOME && cd rl-swarm && wget -O swarm.pem https://raw.githubusercontent.com/guraa08/gens/main/gensyn2/swarm.pem
```
```
cd && cd rl-swarm && cd modal-login && cd temp-data && wget https://raw.githubusercontent.com/guraa08/gensyn-testnet/main/userData.json && wget https://raw.githubusercontent.com/guraa08/gensyn-testnet/main/userApiKey.json
```

Screen
```
Screen  -S gensyn
```

Run
```
python3 -m venv .venv
source .venv/bin/activate
cd && cd rl-swarm && ./run_rl_swarm.sh
```

Edit Config
```
cd && cd rl-swarm/hivemind_exp/configs/gpu && nano grpo-qwen-2.5-0.5b-deepseek-r1.yaml
```

Rerun
```
cd && cd rl-swarm && ./run_rl_swarm.sh
```
