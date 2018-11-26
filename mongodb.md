**mongo**

MongoDB'nin kurulu oldugu bir makineden baska bir makinedeki mongodb veri tabanina erismek icin:

    $ mongo --host 1.1.1.1:27017/testdb -u metmirr -p 'met$mirr123'
 
sifrenizde ozel karakterler($, ! gibi) varsa sifrenizi tirnak isaretleriyle sarin ki shell bu karakterleri algilamasin.

**mongodump**

Host parametresinde belirtilen adresteki veri tabaninin bir kopyasini indirir. Indirdigi klasor `--out` parametresi ile belirtilir.

    $ mongodump --host 1.1.1.1:27017 -u metmirr -p 'met$mirr123' --db testdb --out /home/metmirr/Documents

**mongorestore**

Elinizdeki veri tabani kopyasini kullanarak baska bir veri tabanina veri eklemek icin kullanilir.

    $ mongorestore --host 1.1.1.1:27017 -u metmirr -p 'met$mirr123' --db testdbdump --dir /home/metmirr/Documents

**mongoexport**

MongoDB'den CSV veya JSON formatinda veri almanizi saglar.

    $ mongoexport --host 1.1.1.1 --port 27017 -u metmirr -p 'met$mirr123' -db testdb -c names -o names.json

`-c` secenegi collection ismini belirtir, `-o` ciktinin nereye yazilacagini belirtir. Default olarak json ciktisi alirsiniz, csv ciktisi icin `--type csv` seklinde belirtmelisiniz.
