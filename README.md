<h1 align="center"> RISC Zero Ceremony
 <br/> <br>
 
![image](https://pbs.twimg.com/media/GLfEx-rbUAAYY6-?format=png&name=small)

## Sistem gereksinimleri:
### Ubunutu 22.04
NODE TİPİ | CPU     | RAM      | SSD     |
| ------------- | ------------- | ------------- | -------- |
| RISC Zero  | 2          | 4        | 80 GB |
  

## Kurulum
> Ceremony node çalıştırma değildir. Bu nedenle herhangi bir sunucu da olabilir. Yada yukarıdaki özelliklerde olan bir tanesi yeterli olur.

> Ceremony sırası yoğun olduğu için 20 gün veya daha fazla sürebilir. O nedenle 1 ay gibi düşünebilirsiniz.

> Herhangi çalıştırdığınız sunucu yanına da kurabilirsiniz.
### Güncelleme

```
sudo apt update
sudo apt upgrade -y
```

### NVMI Yüklüyoruz.
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh | bash
source ~/.bashrc
```

### Dizin oluşturuyoruz.
```
mkdir ~/p0tion-tmp
```
```
cd ~/p0tion-tmp
```

### Version nvm v16.20

```
nvm install 16.20
```

```
nvm use 16.20
```

### phase2cli kuralım

```
npm i @p0tion/phase2cli
```

## Github Hesabını Doğrulama.

> [BURADAN](https://github.com/login/device) Yeni sayfada linki açalım. Sonrasında aşağıdaki kodu çalıştırıyoruz.

```
npx phase2cli auth
```

> Size 8 Haneli bir kod verecek.

![Ekran görüntüsü 2024-04-21 171129](https://github.com/CoinHuntersTR/RISC-Zero/assets/111747226/eb44457f-7a49-4402-b627-25919f76a298)

> Bu kodu kopyalıyoruz ve Yukarıdaki açtığımız linke geliyoruz.

![Ekran görüntüsü 2024-04-21 171143](https://github.com/CoinHuntersTR/RISC-Zero/assets/111747226/b4f4c168-68b9-4d7d-9ef2-a295e7643842)

> O kodu githuba giriyoruz. İşlemi doğru yaptığınızda aşağıdaki gibi bir uyarı almanız gerekiyor.

![Ekran görüntüsü 2024-04-21 171157](https://github.com/CoinHuntersTR/RISC-Zero/assets/111747226/530580d5-35de-43a6-bf99-f9b4ffa235d9)

> Terminal Sayfanızda kendi github kullanıcı adınızı görmeniz gerekiyor.

![Ekran görüntüsü 2024-04-21 171206](https://github.com/CoinHuntersTR/RISC-Zero/assets/111747226/a34a8ed9-9a80-42f5-ab47-5e5ba37540b5)

## Ceremony Bölümü

> Öncelikle bir screen açalım.

```
screen -S ceremony
```

> Eğer screen de hata alırsanız. `sudo apt install screen` çalıştırıp sonrasında yukarıdaki komutu tekrar çalıştırın.


```
npx phase2cli contribute
```

> Yukarıki komutu çalıştırdığınızda ilk olarak aşağıdaki gibi bir soru ile karşılaşıyorsunuz. ENTER diyerek geçiyoruz.

![Ekran görüntüsü 2024-04-21 172216](https://github.com/CoinHuntersTR/RISC-Zero/assets/111747226/8598a151-57ed-4d01-8e94-a72f01c245e3)

> İkinci soruya ise Randomly seçiyoruz ve ENTER olarak devam ediyoruz. (Default olarak öyle geliyor, ENTER diyerek devam edebilirsiniz.)

 ![Ekran görüntüsü 2024-04-21 172228](https://github.com/CoinHuntersTR/RISC-Zero/assets/111747226/89d70091-0ac5-4e94-9177-fd5a70e7b843)

> Bu adımlardan sonra aşağıdaki gibi bir sonuç alıyoruz. Gördüğünüz gibi 96 gün gibi bir süre vermiş ve 2870 kişi var önümde o nedenle ara ara kontrol etmek gerekiyor.

![Ekran görüntüsü 2024-04-21 172243](https://github.com/CoinHuntersTR/RISC-Zero/assets/111747226/e12a7621-5c4f-4eab-bad4-8cb0c48e63ca)

### Hatırlatmalar

> Screen içine tekrar girmek için, 

```
screen -r ceremony
```
> Screen içinden çıkmak için CTRL A D ile çıkabilirsiniz.

> Ceremony sırasında durmuş ise, yada siz yanlışlıkla durdurmuşsanız. `npx phase2cli contribute` komutunu tekrar çalıştırabilirsiniz.



 


