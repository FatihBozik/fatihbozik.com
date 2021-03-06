---
layout: post
title: Sürüm Kontrol Sistemleri(Version Control Systems) Hakkında
tags: [version control systems, git]
category: muhtelif
abstract: Sürüm Kontrol Sistemleri nedir? Tarihçesi hakkında
comments: true
---

Sürüm kontrol sistemleri, dosyalar üzerinde yaptığımız değişiklikleri kayıt altına almamıza ve daha sonra bu kayıtlara geri dönebilmemize olanak sağlayan sistemlerdir.<!--mode-->Sürüm kontrol sistemlerini kullanarak

* projenin geçmişteki bir sürümüne erişebilir,
* yapılan değişiklikleri karşılaştırabilir,
* bir dosya üzerinde en son kimin değişiklik yaptığını görebilir,
* bir hata yaptığımızda hataları geri alabiliriz.

## Sürüm Kontrol Sistemlerinin Tarihçesi

### Yerel Sürüm Kontrol Sistemleri(Local Version Control Systems)

Dosyalardaki bütün değişiklikleri(dosya sürümlerini) veritabanına kaydeden sürüm kontrol sistemleridir.

<img style="max-width: 100%;" src="/images/sürüm-kontrol-sistemleri/local version control systems.png" alt="Local Control Systems" height="auto">

### Merkezi Sürüm Kontrol Sistemleri(Centralized Version Control Systems)

İlerleyen zamanlarda programcıların birlikte çalışması ihtiyacı önemli bir sorun olarak karşımıza çıktı. Bu sebeple `Merkezi Sürüm Kontrol Sistemleri`(CVS, Subversion ve Perforce) adı verilen sürüm kontrolüne alınan bütün dosyaların bir sunucuda tutulduğu sistemler geliştirildi. Bu sistemde kullanıcılar sunucudan istedikleri dosyaları seçerek(checkout) kullanırlar.

<img style="max-width: 100%;" src="/images/sürüm-kontrol-sistemleri/centralized version control systems.png" alt="Centralized Version Control Systems" height="auto">

### Dağıtık Sürüm Kontrol Sistemleri(Distributed Version Control Systems)

Yerel ve merkezi kontrol sistemlerinin ikisinde de sürüm kontrolüne alınan dosyalar tek bir bilgisayarda tutulduğundan yedekleme yapılmadığı takdirde merkezi veritabanının sabit diskinde meydana gelebilecek bir hata tüm projenin kaybedilmesine yol açabiliyordu. Bu sorunun çözebilmek için `Dağıtık Sürüm Kontrol Sistemleri`(Git, Mercurial) geliştirildi. Bu sistemlerde istemciler dosyaların yalnızca belelk kopyalarını almakla kalmazlar. Yazılım havuzunu(repository) kopyalarlar. Kullanıcıların yaptığı her seçme işlemi(checkout) bütün verinin yedeklenmesiyle sonuçlanır.

<img style="max-width: 100%;" src="/images/sürüm-kontrol-sistemleri/distributed version control systems.png" alt="Distributed Version Control Systems" height="auto">

<br/><br/><br/><br/>

**Kaynaklar:**

* [Chacon, S. 2009. Pro Git (1st edition)](http://www.amazon.com/Pro-Git-Scott-Chacon/dp/1430218339) <br/>
* https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control
