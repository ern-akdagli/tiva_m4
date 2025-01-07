# tiva_m4
TM4C123GXL Mikrodenetleyici Projeleri

Bu repo, TM4C123GXL mikrodenetleyicisiyle yapılan çeşitli uygulamaları içerir. Projeler, UART iletişimi, ADC kullanımı ve LCD ekran sürme gibi temel mikrodenetleyici işlevlerine odaklanmaktadır. Proje dosyaları ve açıklamalar, kullanıcıların bu mikrodenetleyici ile çalışmayı öğrenmesine yardımcı olmayı amaçlar.

İçerik

1. LCD Ekran Sürme
Açıklama: LCD ekranı 4-bit modda kullanarak veri yazdırma ve konum ayarlama işlemleri yapılmıştır.
Özellikler:
LCD'ye saat (HH:MM:SS) formatında veri yazdırma.
LM35 sıcaklık sensöründen alınan ADC verilerinin °C cinsinden LCD'ye yazılması.
Önemli Fonksiyonlar:
LCD_init(): LCD ekranın başlatılması.
LCD_SetCursor(row, col): İmlecin LCD'deki satır ve sütun konumunu ayarlama.
LCD_Print(str): Karakter dizisini ekrana yazdırma.
2. ADC Kullanımı
Açıklama: LM35 sıcaklık sensörü ile ADC kullanımı yapılmıştır. Sensörden alınan analog veriler, dijitale dönüştürülerek sıcaklık bilgisi hesaplanmıştır.
Önemli Detaylar:
LM35'in ADC üzerinden gelen verilerinin işlenmesi.
ADC kesmeleriyle sıcaklık hesaplama.
Önemli Fonksiyonlar:
adckesmesi(): ADC kesme fonksiyonu, sıcaklık verisini işler.
3. UART İletişimi
Açıklama: Bilgisayardan alınan ve gönderilen verilerin UART üzerinden işlenmesi.
Özellikler:
Bilgisayardan # ve * karakterleriyle birlikte gönderilen tur ve yükseklik bilgilerini okuma.
"bitti" gibi mesajların UART üzerinden gönderilmesi.
Önemli Fonksiyonlar:
sendChar(c): Tek bir karakteri UART üzerinden gönderir.
processData(): Gelen UART verilerini ayrıştırarak tur ve yükseklik bilgilerini alır.
Gereksinimler

Geliştirme Kartı: EK-TM4C123GXL (Tiva C LaunchPad)
IDE: Code Composer Studio (CCS) veya Keil uVision


Projeyi Kopyalayın:
https://github.com/ern-akdagli/tiva_m4

İletişim

Sorularınız veya önerileriniz için lütfen erenakdegli653@hotmail.com üzerinden iletişime geçin.


