**chery-pick** 

Komut bir branch'ten bir comit seçip başka bir branch'e eklemenizi sağlar. Örnek olarak **A** branch'inde çalıştığınızı 
varsayalım ve **B** branch'ınden **9772dd** hash'li commit'i almak istiyorsunuz o zaman:

    $ git cherry-pick <commit hash>
    $ git cherry-pick 9772dd

**status**

Git deponuzdaki değişiklikleri gösterir. Yeni oluşturulmuş dosyalar/klasörler, düzenlenmiş olanlar veya silinmiş olanlar burada görüntülenir.

    $ git status
 
**farklı git geçmişlerine sahip olma problemi**
Eğer birden fazla remote ile çalışıyorsanız bir remote'taki history ile diğerindeki farklı olabilir çünkü siz çalışırken muhtemelen birinden klonlayarak çalışmaya başlamışsınızdır. Örnek olarak ben söyle bir problem yaşadım:

Benim iki tane remote'um vardı biri *remote-a* diğeri *remote-b* ben projeyi klonlarken remote-a'dan klonlayıp `dev` isminde bir branch oluşturdum. Uzun bir zaman hep böyle çalıştım. Ve sonunda remote-a daki dev branch'ını master ile merge'ledim. Aynısını remote-b de yapmaya çalışınca bu branch'lerin tamamen farklı geçmişlere sahip olduklarını söyledi ve merge'leyemediğimi söyledi. Tabi bunu github arayüzünde pull request açmak isterken gördüm. Aynı 
