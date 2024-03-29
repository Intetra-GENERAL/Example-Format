# Örnek Github Formatının Kullanımı

Bu doküman Github reposu oluşturulurken kullanılacak dosyalama standartlarını belirlemek amacıyla oluşturulmuştur.

## Backup Klasörü

Bu klasör içerisinde projenin geliştirme sürecinden kullanılan config , init , backup vb. dosyaları bulunmaktadır.

> [!NOTE]
> Projenin kaynak kodları backup klasörüne atılmamalıdır.

## Documents Klasörü

Bu klasör içerisinde proje sürecinde geliştirilen ve oluşturulan dokümanlar bulunmaktadır. User manuel , teknik dokümanlar , proje raporları gibi dokümanlar bu klasör içerisinde yer alır.

> [!NOTE]
> Bu klasör içerisinde sadece geliştirme sürecinde developer tarafından oluşturulan dokümanlar bulunmalıdır.

## Resources Klasörü

Bu klasör içerisinde proje sürecinde kullanılan dışarıdan edinilen kaynaklar bulunmaktadır. Örneğin proje sürecinde kullanılan görseller , fontlar , css dosyaları , PCB çizimleri gibi kaynaklar bu klasör içerisinde yer alır.

## Source Klasörü

Bu klasör içerisinde proje sürecinde geliştirilen kaynak kodlar bulunmaktadır. Proje sürecinde kullanılan tüm kaynak kodlar bu klasör içerisinde yer alır.

> [!NOTE]
> Birden fazla kaynak kodunun aynı başlık altında toplanması için alt klasörler oluşturulmalıdır.

## ChangeLog.md

Bu dosya içerisinde projenin geliştirme sürecinde yapılan değişiklikler belirtilir. Değişiklikler tarih ve saat bilgisi ile birlikte belirtilir.
Son gönderilen commit ile birlikte versiyon numarası belirtilir ve en üstte yer alır.

## Versiyon Numaralandırma Kuralları

Proje versiyon numaralandırma kuralları aşağıdaki gibidir.

`v.a.b.c.d`şeklinde numaralandırma yapılacaktır.

- a : Projenin baştan sona mimari değişiklikler yapıldığında artar.
- b : Projenin yeni özellikler eklediğinde artar.
- c : Projenin mevcut özelliklerinde değişiklik yapıldığında artar.
- d : Projenin hata düzeltmeleri yapıldığında artar.

```markdown
Release versiyona geçilene kadar sürekli olarak d artar.Release versiyona geçildiğinde a,b,c sıfırlanır ve d artar.

Örneğin : v.0.0.0.1
: v.0.0.0.2
: v.0.0.0.3
: v.0.0.0.4
: ...
: ...
: ...
: ...
: v.1.0.0.0 (Release versiyonu)
: v.1.0.1.0 (Projenin mevcut özelliklerinde değişiklik yapıldı)
```
