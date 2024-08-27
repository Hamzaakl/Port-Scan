
# Basit Port Tarayıcı

Bu Python scripti, belirtilen bir IP adresi üzerinde basit bir port taraması gerçekleştirir. 1 ile 100 arasındaki portlara bağlanmaya çalışır ve hangi portların açık olduğunu raporlar.

## Nasıl Çalışır?

Script, Python `socket` kütüphanesini kullanarak her bir porta TCP bağlantısı oluşturur. Eğer bağlantı başarılı olursa, o port "açık" olarak tanımlanır. Eğer bağlantı başarısız olursa, port "kapalı" olarak işaretlenir.

## Kullanım

1. Scriptte taranacak IP adresini belirtin (`ip` değişkeni).
2. Tarama yapılacak port aralığını (`range(1,100)`) ayarlayın. Varsayılan olarak 1 ile 100 arası portlar taranır.


```bash
python port_scanner.py
```

### Çıktı Örneği

Script çalıştırıldığında, açık ve kapalı portlarla ilgili şu şekilde bir çıktı verir:

```
1 closed
2 closed
3 : open
...
```


