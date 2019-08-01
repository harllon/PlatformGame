# Platform Game

O objetivo desse jogo é fazer com que o personagem atravesse de uma ilha a outra, utilizando as plataformas colocadas no caminho. Essas plataformas têm movimentos aleatórios dentro dos possíveis casos, que são: translação, rotação e escala. Cada plataforma pode ter somente 1 movimento ou uma combinação deles. Os objetos de cenário são da Standard Assets, os quais são montados à maneira do criador, e o personagem também pertence a esse asset.


Segue abaixo uma imagem do ambiente criado, assim como um link para o vídeo que mostra a movimentação das plataformas.

![ambiente](https://user-images.githubusercontent.com/52334298/62245369-e1c9da00-b3b7-11e9-9233-a70128cddb08.jpg)

[vídeo 1](https://youtu.be/18IjnPUjwkE)

O próximo vídeo mostra a ambientação já sobre a perspectiva do personagem.

[vídeo 2](https://youtu.be/QaSZENLSL-w)

A movimentação das plataformas envolve somente animações, sem a presença de um script. Além disso, alguns scripts foram necessários para a perfeita execução do jogo, sendo eles:

### Scripts

1 - Player se move junto a plataforma:

![attachplay](https://user-images.githubusercontent.com/52334298/62284997-293d7e00-b42b-11e9-81bc-2e690752e3d4.jpg)

Esse script consiste em tornar o personagem um filho da plataforma no instante em que a colisão entre os dois seja detectada. Dessa forma, quando a plataforma se move, o personagem acompanha o movimento.

2 - Personagem volta na ilha inicial após queda na água:

![teletransporta(agua)](https://user-images.githubusercontent.com/52334298/62285600-4d4d8f00-b42c-11e9-814e-7aba4d103cb1.jpg)

Esse script faz com que, no instante em que o personagem toca a água, a sua posição seja reiniciada no vector3 dado na imagem. Dessa forma, devido à coordenada y, o personagem entra em queda livre até a ilha inicial.

3 - Teleporta para última plataforma:

![teletransporta(final)](https://user-images.githubusercontent.com/52334298/62285815-c8af4080-b42c-11e9-8bb5-b5b141db3898.jpg)

Esse script faz com que, no instante em que o personagem toca a plataforma, um contador começa a passar o tempo. Quando esse tempo passa de 10 segundos, o personagem é teletransportado para a última plataforma, sendo esse o único modo de chegar à segunda ilha. Cabe mostrar também o script análogo que foi colocado na primeira plataforma. Ele teletransporta o personagem ao início caso o mesmo passe mais de 5 segundos nela.

![teletransporta(inicio)](https://user-images.githubusercontent.com/52334298/62286003-2f345e80-b42d-11e9-9876-6761150d635e.jpg)


#### Gameplay

Por fim, serão mostrados 2 vídeos do jogo: o primeiro mostra o limite alcançado, tentando passar todas as plataformas, enquanto o segundo mostra como chegar ao outro lado.

[vídeo 3](https://youtu.be/fiAVWvGOhSs)

[vídeo 4](https://youtu.be/ypi8Nhbp0z0)

##### Considerações Finais
Esse projeto tem como objetivo desenvolver conceitos trabalhados durante a disciplina de Sistemas Gráficos 3D. Nesse jogo, foram utilizadas assets da Assets Store, como a Standard Assets. Os scripts citados foram manualmente criados e vários conceitos foram envolvidos durante a elaboração do jogo, como as teorias de hierarquia, animação, iluminação e câmera, entre outros elementos que foram usados durante a implementação do jogo.
