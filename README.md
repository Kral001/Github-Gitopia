# Github-Gitopia
Github'ta oluşturduğunuz bir repoyu Gitopia'ya aktarabileceğiniz bir rehber.

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

- Şimdi Gitopia anahtar adımızı git config'de yapılandıralım.

```
git config --global gitopia.key <YOUR-GITOPIA-KEY-NAME>
```









