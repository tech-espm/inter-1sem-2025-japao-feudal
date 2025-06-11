# Projeto Integrado I - Sistemas de Informação ESPM

<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://raw.githubusercontent.com/tech-espm/misc-template/main/logo.png" alt="Sistemas de Informação ESPM" style="width: 375px;"/></a>
</p>

# Mundo de Minecraft situado no Japão feudal

### 2025-01

## Integrantes
- [Rafael Nascimento](https://github.com/tec-Rafael)
- [Ricardo D'Ávila](https://github.com/tec-ricardo)
- [Pedro Veiga](https://github.com/pedro-veiga18)
- [Gustavo Santana](https://github.com/tec-guga)
- [Mattheus Prado](https://github.com/MatGIT19)

## Descrição do Projeto

O projeto “Japão Feudal” tem como objetivo contar uma história original ambientada na era dos samurais e ninjas, figuras japonesas extremamente conhecidas que influenciaram a cultura global, tanto por histórias quanto por filmes e animações. Para isso, foi criada uma vila japonesa em uma montanha, onde os samurais residem e controlam o comércio da região. Visto isso, os ninjas, que no momento estão em desvantagem econômica, planejam um ataque secreto contra a base de operações dos samurais, e, para isso, contarão com a ajuda de um ser sobrenatural, o rei dos Yokais. O plano dos ninjas é aniquilar a vila dos samurais, contudo, os mesmos não deixarão que isso aconteça sem uma batalha. 

## 2.2 Áreas do mapa

### Morro das cerejeiras
<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/image1.png" alt="Sistemas de Informação ESPM" style="width: 500px;"/></a>
</p>

### Praça Central
<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/image11.png" alt="Sistemas de Informação ESPM" style="width: 500px;"/></a>
</p>

### Templo Principal
<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/image14.png" alt="Sistemas de Informação ESPM" style="width: 500px;"/></a>
</p>

### Arsenal Samurai
<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/image15.png" alt="Sistemas de Informação ESPM" style="width: 500px;"/></a>
</p>

### Sala de Reuniões
<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/image16.png" alt="Sistemas de Informação ESPM" style="width: 500px;"/></a>
</p>

### Mesa de criação
<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/image18.png" alt="Sistemas de Informação ESPM" style="width: 500px;"/></a>
</p>

### Sacada 
<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/image20.png" alt="Sistemas de Informação ESPM" style="width: 500px;"/></a>
</p>

### Entrada Norte
<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/image5.png" alt="Sistemas de Informação ESPM" style="width: 500px;"/></a>
</p>

### Entrada Centro de Trocas
<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/image7.png" alt="Sistemas de Informação ESPM" style="width: 500px;"/></a>
</p>

### Centro de Trocas
<p align="center">
    <a href="https://www.espm.br/cursos-de-graduacao/sistemas-de-informacao/"><img src="https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/image9.png" alt="Sistemas de Informação ESPM" style="width: 500px;"/></a>
</p>

## 3 Desenvolvimento

O código foi implementado através da linguagem python e do modelo de programação por blocos do Minecraft Education.

Código da bola de neve (shuriken):
def on_item_interacted_snowball():
	mobs.apply_effect(POISON, mobs.target(NEAREST_PLAYER), 10, 1)
player.on_item_interacted(SNOWBALL, on item_interacted_snowball)

Explicação:
Trecho: “ def on_item_interacted_snowball(): ”, define o que deve acontecer quando um jogador interage com a bola de neve.
Trecho: “ mobs.apply_effect(POISON, mobs.target(NEAREST_PLAYER), 10, 1) ”, aplica efeito de envenenamento no jogador mais próximo, com duração de 10 segundos e amplificação de nível 1. 
Trecho: “ player.on_item_interacted(SNOWBALL, on_item_interacted_snowball) ”, relaciona a definição do que deve acontecer ao interagir com a bola de neve, com a bola de neve e o jogador.

Código da carga de vento (bomba de fumaça):
def on_item_interacted_wind_charge():
	mobs.teleport_to_position(mobs.target(LOCAL_PLAYER), pos_local(1, 3, 5))
	mobs.spawn_particle(SMOKE_CAMPFIRE, pos(0, 0, 0))
	mobs.spawn_particle(SMOKE_BASIC, pos(0, 0, 0))
	mobs.spawn_particle(SMOKE_CAMPFIRE_TALL, pos(0, 0, 0))
	mobs.spawn_particle(SMOKE_LLAMA_SPIT, pos(0, 0, 0))
player.on_item_interacted(WIND_CHARGE, on item_interacted_wind_charge)

Explicação:
Trecho: “ def on_item_interacted_wind_charge(): ”, define o que deve acontecer quando um jogador interage com a carga de vento.
Trecho: “ mobs.teleport_to_position(mobs.target(LOCAL_PLAYER), pos_local(1, 3, 5)) ”, teleporta o jogador para uma posição, em relação a original, 1 bloco ao lado, 3 blocos a cima e 5 blocos a frente. 



Trechos: “ mobs.spawn_particle(SMOKE_CAMPFIRE, pos(0, 0, 0)) ”
	“ mobs.spawn_particle(SMOKE_BASIC, pos(0, 0, 0)) ”
	“ mobs.spawn_particle(SMOKE_CAMPFIRE_TALL, pos(0, 0, 0)) ”
	“ mobs.spawn_particle(SMOKE_LLAMA_SPIT, pos(0, 0, 0)) ”
aplicam diferentes partículas para o efeito da carga de vento, e essas partículas são criadas no local que foi lançada a carga de vento, por isso a posição 0, 0, 0.

Trecho:“player.on_item_interacted(WIND_CHARGE, on_item_interacted_wind_charge)”, relaciona a definição do que deve acontecer ao interagir com a carga de vento, com a carga de vento e o jogador.

## 4 CONCLUSÕES
O projeto teve como principais objetivos aprender a trabalhar em equipe e introduzir o
mundo da tecnologia, de forma engajadora, através do Minecraft, no começo do curso de Ciências de Dados e Negócios da ESPM. Nesse âmbito, conclui-se que nosso trabalho alcançou esses objetivos de forma completa devido a alguns fatores, em destaque o escopo do projeto e a sua natureza.
Como o trabalho foi planejado para um semestre inteiro, ele apresentou diversos requerimentos, como a criação de texturas para itens e blocos, construção de um mapa inteiro, formulação de um roteiro, documentação, gravação de vídeo e codificação. Devido a quantidade de etapas que precisavam ser realizadas, foi necessária a cooperação de todos os integrantes do grupo, de forma que o trabalho ficasse dividido igualmente para todos e para que então ele tomasse forma constantemente ao longo das semanas. Foi uma experiencia única para conhecer os participantes do grupo e considerar diversas visões sobre o projeto, e isso não teria acontecido caso o projeto fosse menor em escala e tempo.
Além disso, a natureza do trabalho foi essencial para introduzir o mundo da tecnologia, pois Minecraft é um jogo que é majoritariamente conhecido por todos os participantes devido a sua presença forte na infância de muitos. Ademais, ele é um jogo de fácil acesso e fácil manipulação, quando comparado com outras opções do mercado, então a escolha dele para a realização do projeto foi excelente.
Devido a esses fatores principais, conclui-se que os principais objetivos foram alcançados e que o projeto foi realizado de forma completa, com a participação de todos os integrantes.

# Licença

Este projeto é licenciado sob a [MIT License](https://github.com/tech-espm/inter-1sem-2025-japao-feudal/blob/main/LICENSE).
