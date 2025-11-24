### verkefni 1a
```bash
Sláðu inn tölu a: 7 

Sláðu inn tölu b: 8 

a + b = 15
```
### verkefni scripts
```bash
#!/bin/bash

echo "Hvaða margföldunar töflu viltu"
read MTAFLA
if [ $MTAFLA -ne 0 ]
then
 for tala in {1..10}
        do
        echo "$tala xx $MTAFLA =" $(($tala * $MTAFLA))
        done

else
 for t in {0..10}
        do
        for tala in {1..10}
                do
                echo "$t x $tala =" $(($tala * $t))
                done
        done

fi
```
### Tímaverkefni 2b
```bash
echo "Hvaða sveitarfélag viltu skoða:"
read NAME
COUNT=$(grep $NAME fakenames.csv | wc -l)
echo Í sveitarfélaginu Akureyri eru $COUNT skráðir.
```
