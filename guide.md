![alt text](https://i.hizliresim.com/6980i8v.png)

# Hatırlatma

İlk ağ oluşumuna, node kurulum testine ve protokol performans ölçümüne odaklanan 1 haftalık bir early alfa test ağı aşaması yürütecekler.
12 Eylül'den önce her zaman kurabilirsiniz. Form gönderim ve onaylama olduğundan erken kurmakta fayda olacaktır.

- **5 Eylül 2023: Testnet Başlangıcı** 
- **8 Eylül 23:00: Node Community Call**
- **12 Eylül: Testnet Optimizasyonunun Kapatılması**
- **14 Eylül:Geri bildirim, veri sonuçlarını ve kalıcı testnet spin-up tahminleri.**

# Minimum Sistem Gereksinimleri

- **4 CPU**
- **32GB RAM**
- **20GB DISK**
- **Ubuntu 22.04+**

16GB Ram'de hata verecek ama yine devam edebiliyorsunuz. 

```python
sudo apt update && sudo apt upgrade -y
```


```python
sudo apt install curl tar wget clang pkg-config libssl-dev jq build-essential bsdmainutils git make ncdu gcc git jq chrony liblz4-tool -y
```

```python
curl https://get.fleek.network | bash
```

Eğer 16GB RAM kullanırsanız aşağıdaki gibi bir hata alacaksınız. Enter yaparak devam edebilirsiniz.

![alt text](https://i.hizliresim.com/ad5gmgq.png)

Eğer 32GB RAM kullanıyorsanız hata vermeyecek.


![alt text](https://i.hizliresim.com/tqz27hc.png)

Kurulum biraz uzun sürebilir. Kurulum bittikten sonra firewall hatası alırsanız aşağıdaki gibi bir çıktı göreceksiniz.

![alt text](https://i.hizliresim.com/ol7tdnc.png)

Bu durumda tekrar sunucuya bağlanıp aşağıdaki kodu girin ve sonra diğer sunucu bağlantınızda Enter yapın.

```python
ufw disable
```

![alt text](https://i.hizliresim.com/d1rozv4.png)

Yukarıdaki çıktı da Node Public Key ve Consensus Public Key çıktılarını kaydedin. 

/root/.lightning/keystore dizinindeki keystore dosyasını sftp bağlantısı ile bilgisayarınıza indirin.

![alt text](https://i.hizliresim.com/m7k1ro4.png)



Çıktıdaki gibi uyarı alacaksınız. Node'unuzu gerekli bilgileri girerek form ile göndermeniz gerekiyor. 

![alt text](https://i.hizliresim.com/eg3om5z.png)

Form için Fleek Discord'unda access-form kanalında aşağıda gösterildiği gibi bilgilerinizi girin. 


![alt text](https://i.hizliresim.com/7rehvjp.png)

![alt text](https://i.hizliresim.com/p2ywll6.png)

Ağ başlatma, durdurma veya restart

```python
systemctl start lightning
systemctl stop lightning
systemctl restart lightning
```


Status çıktısı

```python
systemctl status lightning
```

Node çıkışı 

```python
tail -f /var/log/lightning/output.log
```

Diagnostics

```python
tail -f /var/log/lightning/diagnostic.log
```

Şu an takım formu daha kabul etmediği için yukarıdaki kontrol kodlarından sonra aşağıdaki gibi çıktılar çıkacaktır. 

![alt text](https://i.hizliresim.com/6dwtcob.png)


Node Public Key ve Consensus Public Key çıktısı

```python
lgtn keys show
```

![alt text](https://i.hizliresim.com/en9uqkx.png)



- **https://t.me/testnetrun**

- **https://link3.to/testnetrun**

- **https://www.youtube.com/@TestNetRun**

- **https://testnet.run/**

- **https://stake.testnet.run/**

- **https://twitter.com/testnetrun**





