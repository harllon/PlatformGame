# Platform Game

## Projeto do curso XXXXX 2019

O objetivo desse jogo é atravessar de uma ilha a outra, utilizando as plataformas colocadas no caminho.
Essas plataformas tem movimentos aleatórios dentro dos possíveis casos, são eles: translação, rotação e escala.
Cada plataforma pode ter somente 1 movimento ou uma combinação deles. Os objetos de cenário são da Standard Assets, sendo montados a maneira do criador, o personagem também pertence a esse asset.


Seguem abaixo uma imagem do ambiente criado assim como um link para o video que mostra a movimentação das plataformas.

![ambiente](https://user-images.githubusercontent.com/52334298/62245369-e1c9da00-b3b7-11e9-9233-a70128cddb08.jpg)

https://www.youtube.com/watch?v=18IjnPUjwkE

O próximo vídeo mostra a ambientação já sobre a perspectiva do personagem.

https://youtu.be/QaSZENLSL-w

A movimentação das plataformas envolvem somente animações, sem a presença de um script. Além disso, alguns scripts foram necessários para a perfeita execução do jogo sendo eles:

###Scripts

1. Player se move junto a plataforma:

(imagem)

Esse script consiste em, tornar o personagem um filho da plataforma no instante em que a colisão entre os dois seja detectada. Dessa forma, quando a plataforma se move, o personagem acompanha o movimento.

2. Personagem cai na ilha inicial após queda na água:

(imagem)

Esse script faz com que no instante em que o personagem toca a água, a sua posição seja reiniciada no vector3 dado na imagem. Dessa forma, devido a coordenada y, o personagem entra em queda livre até a ilha inicial.

3. Teleporta para última plataforma:
(imagem)

Esse script faz com que, no instante em que o personagem toca a plataforma um contador começa a passar o tempo. Quando esse tempo passa de 10 segundos o personagem é teletransportado para a última plataforma, sendo este o único modo de chegar a segunda ilha.
Cabe mostrar também o script análogo que foi colocado na primeira plataforma. Ele teletransporta o personagem ao inicio caso o mesmo passe mais de 5 segundos nela.

(imagem)

####Gameplay

Por fim, serão mostrados 2 vídeos do jogo, o primeiro mostra o limite alcançado tentando passar todas as plataformas, enquanto o segundo mostra como chegar ao outro lado.

https://youtu.be/gXkUWRJ3-XE

https://youtu.be/ypi8Nhbp0z0

#####Considerações finais
Esse projeto tem como objetivo desenvolver conceitos trabalhados durante a disciplina de Sistemas Gráficos 3D. Nesse jogo foi utilizada assets da Assets Store como a Standard Assets. Os scripts citados foram manualmente criados e vários conceitos foram envolvidos durante a elaboração do jogo, como a teoria de hierarquia, animação, iluminação e câmera, entre outros elementos que foram usados durante a implementação do jogo.
