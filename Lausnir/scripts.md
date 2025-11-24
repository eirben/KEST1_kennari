### verkefni 1a
```bash
#!/bin/bash

echo "Sláðu inn tölu a:"
read a
echo "Sláðu inn tölu b:"
read b
echo "a + b = $(($a + $b))"
```
### verkefni1b
```bash
#!/bin/bash
echo "Aðgerðir:"
echo "1: a + b"
echo "2: a – b"
echo "Veldu aðgerð"
read TYPE
echo "Sláðu inn tölu a:"
read a
echo "Sláðu inn tölu b:"
read b
if [ $TYPE -eq 1 ]
then
        echo "$a + $b = "$(($a + $b))
else
        echo "$a - $b = "$(($a - $b))
fi
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
