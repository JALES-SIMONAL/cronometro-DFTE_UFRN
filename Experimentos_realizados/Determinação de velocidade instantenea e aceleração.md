
# Determinação de velocidade instantenea e aceleração
O presente experimento foi tem o objetivo de verificar a aceleração instantanea de um carro em 2 pontos sobre um trilho de ar( sem atrito).

## Descrição da montagem do experimento 

A [imagem](#layout) abaixo mostra a disposição da montagem. A montagem consiste em um trilho de ar com [inclinação de 5°](#medição_graus_inclinação) conectado a um soprador de ar. Na extremidade esquerda do trilho de ar, encontra-se um disparador mecânico manual, responsável por iniciar o movimento. Logo à frente do disparador mecânico se encontra o carro, que se movimentará de uma ponta a outra do trilho após o disparo. Sobre o carro, há uma vela com comprimento de [10 cm](#mediçãoVela), usada para calcular a velocidade instantânea nos dois pontos escolhidos. Os sensores *photogate* S1 e S2 usados são de [fabricação própria](#sensor) e foram posicionados respectivamente nas posições [140cm ](#s1_140) e [90cm](#s2_90). Os sensores *photogate* têm sua alimentação e seu sinal de resposta conectados ao hardware de aquisição de dados.

<br><br>
<div id="layout" align="center">
  <img src="https://github.com/user-attachments/assets/6b5d8857-9b4a-444d-88c9-55b7df2beb25" alt="bancada_teste_experimento" width="600"/>
  <br>
  <em>Bancada de teste do experimento</em>
</div>

## medições dos tempos

### Velocidade Instantânea no Sensor S1

| $t_1$ (ms) | $t_2$ (ms) | $t_2 - t_1$ (ms) | Velocidade instantânea (m/s) |
| :---: | :---: | :---: | :---: |
| 3329 | 3425 | 96 | 1,041666667 |
| 4083 | 4176 | 93 | 1,075268817 |
| 4557 | 4650 | 93 | 1,075268817 |
| 4602 | 4700 | 98 | 1,020408163 |
| 4584 | 4682 | 98 | 1,020408163 |
| 4563 | 4657 | 94 | 1,063829787 |
| 2734 | 2832 | 98 | 1,020408163 |
| 3691 | 3788 | 97 | 1,030927835 |
| 2824 | 2919 | 95 | 1,052631579 |
| 5798 | 5898 | 100 | 1 |
| 1617 | 1706 | 89 | 1,123595506 |
| **Velocidade média em S1** | | | **1,15244135** |

### Velocidade Instantânea no Sensor S2

| $t_1$ (ms) | $t_2$ (ms) | $t_2 - t_1$ (ms) | Velocidade instantânea (m/s) |
| :---: | :---: | :---: | :---: |
| 3757 | 3832 | 75 | 1,333333333 |
| 4501 | 4575 | 74 | 1,351351351 |
| 4975 | 5049 | 74 | 1,351351351 |
| 5038 | 5115 | 77 | 1,298701299 |
| 5019 | 5095 | 76 | 1,315789474 |
| 4983 | 5058 | 75 | 1,333333333 |
| 3167 | 3243 | 76 | 1,315789474 |
| 3121 | 3197 | 76 | 1,315789474 |
| 3245 | 3320 | 75 | 1,333333333 |
| 6241 | 6318 | 77 | 1,298701299 |
| 2018 | 2089 | 71 | 1,408450704 |
| **Velocidade média em S2** | | | **1,465592443** |

## calculos

$$v_{s2}^2 = v_{s1}^2 + 2a\Delta s$$

$$a = \frac{v_{s2}^2 - v_{s1}^2}{2\Delta s}$$

$$a = \frac{1,465592^2 - 1,152441^2}{2 \cdot 0,5} = 0,819 \text{ m/s}^2$$

$$a = g \cdot \sin(\theta)$$

$$a = 9,81 \cdot \sin(5^\circ) \approx 0,854 \text{ m/s}^2$$

<br><br>

## Imagens das medições

<div id="medição_graus_inclinação" align="center">
  <img src="https://github.com/user-attachments/assets/84fcf58d-6338-43c9-abe7-39a81bb3ac94" alt="medicao_inclinacao" width="300"/>
  <br>
  <em>Medição de inclinação, 5° de inclinação
</div>

<br><br>

<div id="mediçãoVela" align="center">
  <img src="https://github.com/user-attachments/assets/2dfd74ce-351b-4942-9695-211e30a84d52" alt="medição_da_vela" width="300" />
  <br>
  <em>Medição da vela, comprimento de 10cm</em>
</div>

<br><br>

<div id="s1_140" align="center">
  <img src="https://github.com/user-attachments/assets/facae6a6-86c1-4c9e-883e-6b8181a24316" alt="posicao_sensor_s1" width="300"/>
  <br>
  <em>Posição do sensor s1 140cm</em>
</div>

<br><br>

<div id="s2_90" align="center">
  <img src="https://github.com/user-attachments/assets/2eb82f9a-d5a6-4b01-a38f-13b6bb0bd79f" alt="posicao_sensor_s2" width="300"/>
  <br>
  <em>Posição do sensor s2 90cm</em>
</div>

<br><br>

<div id="sensor" align="center">
  <img src="https://github.com/user-attachments/assets/f222edff-1653-4469-8fcd-149835c1f742" alt="sensor_photogate_proprio" width="300"/>
  <br>
  <em>sensor photogate de fabricação própria</em>
</div>
