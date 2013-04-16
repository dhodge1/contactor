#!/bin/sh

if [ $1 = '-e' ] ; then
        echo "Fetching emails"
        egrep -o '[a-zA-Z0-9.\-_]+@[a-zA-Z0-9.\-_]+\.(com|org|net|edu)\>' $2
elif [ $1 = '-p' ] ; then
        echo "Fetching phone numbers"
        egrep -o '([0-9]{3}+\-[0-9]{3}+\-[0-9]{4}+\>|\([0-9]{3}+\)[0-9]{3}+\-[0-9]{4}+\>)' $2
else
        echo "Invalid argument."
        echo "Usage ./phoneHome.sh (-e|-p) input_file"
fi
