   cd /opt
   mkdir /opt/Bloodhound
   cd /opt/Bloodhound

Install Docker

sudo apt install docker.io && sudo apt install docker-compose

## Add your user to the doecker group
sudo usermod -aG docker $USER

Install Bloodhound

## download bloodhound docker compose file https://ghst.ly/get
curl -L https://ghst.ly/getbhce > docker-compose.yml

##starting Bloodhound
sudo docker-compose pull && docker-compose up

Getting temp password

admin
nDMeWeebkzF7UxAVWfrCa5FcqdkpBJ3J

### Start Bloodhound 
docker-compose up -d
