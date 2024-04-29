#Step 1: Update docker-compose.yml
sed -i 's/$PT/UTM/g' docker-compose.yml

#Step 2: Docker compose up
docker compose up -d

#Step 3: Docker compose stop
docker compose stop

#Step 4: Display PeerID from ipfs/config (untuk bootstrap)
cat ipfs/config | grep "PeerID"

#Step 5: Display identity.json from cluster (untuk cluster)
cat cluster/identity.json | grep "id"

#Setorkan Peer ID & dan peer cluster ID kedalam excel
#samakan secret key dengan secret key yang ada di excel
nano cluster/service.json

#masukan alamat bootstrap ipfs
nano bootstrap.sh

#masukan alamat bootstrap ipfs-cluster
nano cluster/peerstore

#docker_start
docker compose start
