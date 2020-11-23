#!/bin/bash
#6-ip.sh
ETH0=`/sbin/ifconfig eth0 | grep netmask | cut -di -f2 | cut -d' ' -f2`
MASK0=`/sbin/ifconfig eth0 | grep netmask | cut -dm -f2 | cut -d' ' -f2`
echo "O endereço de IP da interface ETH0 é $ETH0 e su máscara de rede é $MASK0"
ETH1=`/sbin/ifconfig eth1 | grep netmask | cut -di -f2 | cut -d' ' -f2`
MASK1=`/sbin/ifconfig eth1 | grep netmask | cut -dm -f2 | cut -d' ' -f2`
echo "O endereço de IP da interface ETH1 é $ETH1 e su máscara de rede é $MASK1"