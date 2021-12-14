#! /usr/bin/make -f

jsonld:=../cups_dates.jsonld ../cups.jsonld

jsonld:${jsonld}

${jsonld}:../%.jsonld:%.rq kc.csv
	tarql $*.rq  kc.csv | riot --syntax=ttl --output=jsonld > $@
