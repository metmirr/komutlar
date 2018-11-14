**systemctl**

Linux'de yazdigim servislerden calisanlari listelemek icin:

    $ systemctl | grep running | myservice
  
yukaridaki komut calisan servislerin icerisinden "myservice" kelimesi olan servisleri gosterir.

**scp**

Bir makineden baska bir makineye dosya gondermek veya almak icin kullanilan komuttur.

    $ scp metmirr@1.1.1.1:/home/metmirr/Desktop/names.json Desktop/data/

yukaridaki komut *1.1.1.1* ip adresindeki makineye *metmirr* kullanicisi ile baglanip, */home/metmirr/Desktop/names.json* dizinindeki dosyayi bu komutun yazildigi bilgisayara kopyalar.

**service**

Sisteminizdeki servisleri calistirmak, durdurmak ve durumlarini ogrenmek icin kullanirsiniz:

    $ service mongod status

*mongod* isimli servisin durumunu gosterir.
