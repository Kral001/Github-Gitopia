<h1 align="center"> Github-Gitopia </h1>

- Github'ta oluşturduğunuz bir repoyu Gitopia'ya aktarabileceğiniz bir rehber ile karşınızdayım. O halde haydi başlayalım.

- Bu işlemi gerçekleştirmek için önce Gitopia üzerinde bir repo oluşturmalıyız. Bunun için Gitopia sitesinde profilimize girdiğimizde 'Create a repository' seçeniğine tıklayın.

<img width="1418" alt="1" src="https://user-images.githubusercontent.com/98269269/208249327-e36f37f0-9aff-4094-a546-72f9433a4b97.png">

- Açılan ekranda 'Repository name' ve 'description' kısımlarını dolduralım. Ardından 'Create repository' kısmına tıklayalım.

<img width="1418" alt="2" src="https://user-images.githubusercontent.com/98269269/208249375-83d1b5e1-143b-4056-ba03-dbdcec2e8a31.png">


- Şimdi yapacağımız adımları çok dikkatli yapmalısınız. Öncelikle git remote helper yükleyeceğiz. Bu işlemleri yapabilmek için Gİtopia sunucunuzu açın ve ana terminalde işlem yapın.

- Önce aşağıdaki komut ile kurulumu yapıyoruz.

```
curl https://get.gitopia.com | bash
```
- Yukarıdaki kodu girdiğinizde aşağıdaki hatayı alırsanız, bir sonraki kodu girmelisiniz. Aşağıdaki hatayı almazsanız bir sonraki komutu girmenize gerek yoktur.

![4](https://user-images.githubusercontent.com/98269269/208249557-ae6ee762-5fc0-4e8b-9ab1-0a14f946fbd6.png)

- Yukarı hatayı aldıysanız bu kodu girmelisiniz.
```
sudo mv /tmp/tmpinstalldir/git-remote-gitopia /usr/local/bin/
```


- Şimdi anahtarımızı OS anahtarına ekleyeceğiz. Aşağıdaki komutta yer alan <YOUR_KEY_NAME> kısmına kendiniz için bir isim belirleyip yazıyorsunuz. Ve bu kodu giriyorsunuz.
  
```
git gitopia keys add <YOUR-KEY-NAME> --recover
```
- Yukarıdaki komutu girdiğinizde, cüzdan anımsatıcınızı girmeniz istenecektir. Cüzdanınızın 24 kelimelik kurtarma ifadesini yazın ve ENTER'a basın.

- Kelimeleri girip ENTER tuşuna bastığınızda karşınıza böyle bir çıktı çıkmalı.

![5](https://user-images.githubusercontent.com/98269269/208249849-88c90335-cf64-45dc-b303-0b80b3c800d6.png)

- Şimdi Gitopia anahtar adımızı git config'de yapılandıralım. <YOUR_KEY_NAME> yazan yere biraz önce yukarıda belirlediğiniz adı yazmalısınız.

```
git config --global gitopia.key <YOUR-GITOPIA-KEY-NAME>
```



- Ana adımlara geçmeden önce Keplr cüzdan Mnemonic Seed Phrase'inizi bulmanız gerekiyor. Bunun için öncelikle araç çubuğunuzdaki Keplr uzantı ikonuna tıklayarak hesabınıza giriş yapın ve ardından görseldeki gibi hesap ikonuna tıklayın.

<img width="1420" alt="az" src="https://user-images.githubusercontent.com/98269269/208250010-db70ff75-1925-4258-af8b-67976aee8511.png">

- Şimdi, gösterildiği gibi hesap adınızın yanındaki üç noktayı tıklayın.

<img width="1420" alt="azz" src="https://user-images.githubusercontent.com/98269269/208250050-7d46f096-7e1e-4cdb-8194-5ff8f7e84c42.png">

- Ortaya çıkan seçim menüsünde, View Mnemonic Seed'e tıklayın

<img width="1420" alt="azz" src="https://user-images.githubusercontent.com/98269269/208250170-8bf86f0a-c71c-4942-98bb-501b97902708.png">

- Cüzdan şifrenizi yazmanız istenecektir. Doldurulduktan sonra Confirm tuşuna tıklayın.

<img width="1420" alt="azz" src="https://user-images.githubusercontent.com/98269269/208250231-5c087cf4-0ccf-47e1-8112-c87760a0ee99.png">

- Keplr cüzdanınız Mnemonic Seed Phrase şimdi görüntülenecektir. Anahtarınızı işletim sistemi anahtarlığında ayarlamak için bu anımsatıcıya ihtiyacınız olacak. Bu nedenle bu ifadeleri güvende tuttuğunuzdan emin olmalısınız.

<img width="1420" alt="az" src="https://user-images.githubusercontent.com/98269269/208250281-069b87c5-6eaf-4274-a4fc-6cc9fc49a410.png">

- Oluşturduğunuz anahtarlarınızın isimlerini görmek için aşağıdaki kodu kullanabilirsiniz.

```
git gitopia keys list
```
- Yukarı komutu kullandığınızda aşağıdaki gibi bir çıktı alacaksınız. Bu çıktıda key isimlerinizi görebilirsiniz.

![7](https://user-images.githubusercontent.com/98269269/208250409-ac4822cd-7763-4aba-aa2d-cf9dab8ed79b.png)
