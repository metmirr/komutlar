**mongo**

MongoDB'nin kurulu oldugu bir makineden baska bir makinedeki mongodb veri tabanina erismek icin:

    $ mongo --host 1.1.1.1:27017/testdb -u metmirr -p 'met$mirr123'
 
sifrenizde ozel karakterler($, ! gibi) varsa sifrenizi tirnak isaretleriyle sarin ki shell bu karakterleri algilamasin.
