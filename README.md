## StarkNet, Node Kurulum Kılavuzu Türkçe Çeviri.

(İngilizceden çevrilmiştir, alıntıdır)

# Öncelikle bir Alchemy hesabı oluşturuyoruz.

Starknet'i çalıştırmak için Alchemy hizmeti tarafından sağlanan düğümleri kullanacağız, bu nedenle [alchemy.com](https://www.alchemy.com/)'a kaydolun ve kişisel hesabınızda endpointler oluşturalım.

# Sırasıyla görseller:

![image](https://user-images.githubusercontent.com/101149671/171650488-9846b8e5-d76d-43a7-a256-402cba2e0f8a.png)

![image](https://user-images.githubusercontent.com/101149671/171650517-7b22a87e-fff5-4704-b38b-1464f82e83f2.png)

![image](https://user-images.githubusercontent.com/101149671/171650593-c63e40b7-71c3-4c14-8a69-daf26a066677.png)

![image](https://user-images.githubusercontent.com/101149671/171650619-a0527993-19ec-4ce0-a674-033b68da1cea.png)

![image](https://user-images.githubusercontent.com/101149671/171650653-8eb80d02-d369-4602-9770-cd0d17fa8a06.png)


Görsellerde gösterdiğim şekilde hesabı oluşturun ve adresi kopyalayın.


# KURULUM:

```
ALCHEMY=YOUR_ALCHEMY_HTTP_ADDRESS
echo 'export ALCHEMY='$ALCHEMY >> $HOME/.bash_profile
```

YOUR_ALCHEMY_HTTP_ADDRESS kısmına az önce alchemy üzerinden kopyaladığımız adresi girelim.

# Hızlı kurulum için script:

```
wget -O starknet.sh https://api.nodes.guru/starknet.sh && chmod +x starknet.sh && ./starknet.sh
```

# Logları takip etmek için:

```
journalctl -u starknetd -f
```

# Node restart atmak için:
```
systemctl restart starknetd
```

# Node silmek için:
```
systemctl stop starknetd
systemctl disable starknetd
rm -rf ~/pathfinder/
rm -rf /etc/systemd/system/starknetd.service
rm -rf /usr/local/bin/pathfinder
```

# İşlemler bu kadar, teşekkürler.
```
https://t.me/RuesAnnouncement
https://t.me/RuesChat
https://t.me/RuesNode
https://t.me/RuesNodeChat
https://forum.rues.info/
```



















