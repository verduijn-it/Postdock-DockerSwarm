# Postdock-DockerSwarm
This Project is heavily based on Postdock (https://github.com/paunin/PostDock) and I just maked it Suitable for Docker Swarm and docker-compose with postgis module.

Thanks to (https://github.com/paunin) for his great work


## Installing:

1- Install Docker-ce on all of the participate nodes

2- create your swarm cluster

3- git Clone this repo on /opt/   on every node that is participate in the cluster

4- Set Swarm node tags (based on swarm-cli scripts, for example set pgtype == primary for the node that you want to use as Master Node)

5- Run scripts in the swarm-cli directory on Swarm Manager Node:

    -Run pgmaster ./opt/swarm-cli/run-pgmaster.sh
    
    - then pgslave1 ./opt/swarm-cli/run-pgslave1.sh
    
    - then pgsalve2 ./opt/swarm-cli/run-pgslave2.sh
    
    - then pgpool and pgbackup  ./opt/swarm-cli/run-pgpool.sh  and ./opt/swarm-cli/run-pgbackup.sh
    
    
6- Done.

Please read more about this project on its original repo  (https://github.com/paunin/PostDock)


