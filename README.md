# crabmusket HQ

Experiments in deploying CoreOS.

## Getting in

    ssh-add ~/.ssh/id_rsa
    export FLEETCTL_TUNNEL=$DROPLET_IP
    fleetctl-0.10.2 list-units

## Setting up

    cd bridge
    fleetctl-0.10.2 submit vulcan.service landing@.service
    fleetctl-0.10.2 start landing@1
    fleetctl-0.10.2 start vulcan
