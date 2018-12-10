Bu komutların çalışması için **pipenv**'in yüklü olması gerekmektedir.

Ubuntu: `pip install --user pipenv`

Windows: `pip.exe install pipenv`


**Bir sanal ortam oluşturma**

Sanal ortam, projenizin geliştirmesinde kullanacağınız paketleri sisteminize yüklemek yerine bu sanal ortama kurduğunuz ortama verilen isimdir. Buradaki amaç sisteminize gereksiz veya sisteminizin işleyişini bozacak işlemlerden kaçınmaktır. Python'da sanal ortamlar oluşturmak için birden fazla seçeneğiniz mevcuttur.

Pipenv ile sanal ortam oluşturmak için:

    $ pipenv shell

Yukarıdaki komut bulunduğunuz klasör ile ilişkilendirilmiş bir sanal ortam oluşturur. Bu sanal ortam için kullanılacak Python yorumlayıcısını yükler ve hazır duruma getirir. Bu komuttan sonra artık bu sanal ortamda çalışmaya başlarsınız. Eğer bu komuttan sonra terminali kapatırsanız ve yeni bir terminal acarsanız sanal ortamı aktif etmek için sanal ortamın kurulu olduğu dizine gidip bu komutu çalıştırmalısınız.

Pipenv ile bir sanal ortam oluşturulduğunda pipenv otomatik olarak *Pipfile* isminde bir dosya oluşturur. Bu dosya projeniz için yüklediğiniz paketleri tutar ki başka biri projenizi aldığında hangi paketleri kuracağını bilsin.

Pipenv ile paket yüklemek:

    $ pipenv install flask
    
*flask* ismindeki paketi sanal ortamınıza yükler ve bu paketi Pipfile dosyasına ekler.

Yüklü olan paketleri listelemek için:

    $ pipenv graph
