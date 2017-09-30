---
title: "Failed to resolve: junit:junit:4.12"
categories:
  - muhtelif
tags:
  - android studio gradle error
  - junit error
---

### Hata
Ubuntu işletim sisteminde Android Studio'da yeni bir proje oluşturduğumda karşılaştığım bir hata.

<img style="max-width: 100%;" src="/assets/images/failed-to-resolve-junit/junit error.png" alt="Grandle junit hatası" height="auto">

### Çözüm
`../AndroidStudioProjects/{ProjectName}/app/build.gradle` dosyası aşağıdaki gibi düzenlenir.
{% highlight groovy %}
android {
    ...
    repositories {
        maven { url 'http://repo1.maven.org/maven2' }
    }
}
{% endhighlight %}