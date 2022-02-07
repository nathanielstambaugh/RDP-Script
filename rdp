#!/bin/bash

echo -n "Enter server name: "
read svrname
echo -n "Enter the username: "
read usrname
echo -n "Enter the password: "
read password
echo -n "Please enter the domain(optional): "
read domain

if [ -z "$domain" ]
then
	rdesktop -r clipboard:CLIPBOARD -r disk:HOME=/home/nstambaugh/Desktop -u "$usrname" -p "$password" -f "$svrname"
elif [ -n "$domain" ]
then
	rdesktop -r clipboard:CLIPBOARD -r disk:HOME=/home/nstambaugh/Desktop -u "$usrname" -p "$password" -f "$svrname" -d "$domain"
fi 


