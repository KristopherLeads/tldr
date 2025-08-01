# docker

> Docker konteyner ve imgelerini yönetir.
> `run` gibi bazı alt komutların kendi dökümantasyonu bulunmaktadır.
> Daha fazla bilgi için: <https://docs.docker.com/reference/cli/docker/>.

- Tüm (çalışan veya duran) Docker konteynerlerini listele:

`docker ps {{[-a|--all]}}`

- Bir imgeden özel bir isimle konteyner başlat:

`docker run --name {{konteyner_ismi}} {{imge}}`

- Varolan bir konteyneri başlat veya durdur:

`docker {{start|stop}} {{konteyner_ismi}}`

- Bir Docker kaydından imge çek:

`docker pull {{imge}}`

- Halihazırda çalışan bir konteyner içinde komut istemcisi aç:

`docker exec {{[-it|--interactive --tty]}} {{konteyner_ismi}} {{sh}}`

- Durmuş bir konteyneri sil:

`docker rm {{konteyner_ismi}}`

- Bir konteynerin kaydını çek ve takip et:

`docker logs {{[-f|--follow]}} {{konteyner_ismi}}`
