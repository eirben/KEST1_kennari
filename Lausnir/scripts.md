
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


