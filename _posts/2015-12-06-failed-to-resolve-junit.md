---
layout: post
title: "Failed to resolve: junit:junit:4.12"
tags: [android studio gradle error, junit error]
comments: true
category: muhtelif
image:
  feature:
excerpt_separator: <!--more-->
---

### Hata
Ubuntu işletim sisteminde Android Studio'da yeni bir proje oluşturduğumda karşılaştığım bir hata.

<!--more-->

<img style="max-width: 100%;" src="{{ site.baseurl }}/images/failed-to-resolve-junit/junit error.png" alt="Grandle junit hatası" height="auto">

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
