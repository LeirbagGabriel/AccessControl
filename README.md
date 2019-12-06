# Access Control
O objetivo do projeto é usar um teclado matricial de membrana para realizar o acesso de pessoas em um condomínio. No sistema existem quatro usuários, cada qual com suas respectivas senhas. Para realizar a entrada, primeiramente é necessário a digitação da senha. Se estiver correta, a passagem é liberada e uma mensagem é enviada ao porteiro através de dispositivo bluetooth, informando o titular e apartamento do usuário. Também é possível fazer a redefinição de senhas (com informação ao porteiro por bluetooth), sendo exigida uma senha mestre para verificação de autenticidade. No caso em que houver sucessivas falhas na tentativa de entrada, o sistema será travado, sendo necessária  a presença do porteiro para inserção da senha-mestre, gerando o destravamento do sistema.
Em cada etapa os leds acedem de forma única informando o funcionamento do programa com base na mensagem apresentada ao usuário.
Por exemplo, quando a senha é verificada como correta o led azul acende, indicando que a passagem foi liberada; caso a passagem seja negada, o led vermelho acende; caso ocorra 3 erros consecutivos da senha, o sistema trava e os dois leds ficam ativos.

Aplicações:
Uso geral para controle de entrada de pessoas em diferentes tipos de ambientes, tais como empresas, escolas, condomínios, residências, mostrando assim a versatilidade do sistema, sendo necessária fazer apenas poucas alterações para que ele funcione perfeitamente nesses locais.

Possíveis melhorias:
.Na comunicação Bluetooth-Monitor, poderia ser adicionado também a hora de chegada.
.A implementação de 3 erros para a senha-mestre.
.Utilização de um banco de dados para armazenagem dos dados mais segura.

Problemas Encontrados:
.Não foi possível adicionar mais funcionalidades pois o sistema utiliza 4Bits para enviar dados.
.A implementação da hora de chegada não foi possível pois o a função utilizada não funciona na GreenPill pois excede o espaço da memória flash.


Materiais utilizados:
.STM32F030F4P6 - GREENPILL
.Gravador ST-LINK V2
.oLed
.Teclado matricial 4x4
.Módulo Bluetooth HC-05
.Dois leds
.Protoboard e jumpers


Membros:
Gabriel Castro Marinho              405229
Gabriela Casimiro de Lima           370065
Rodrigo Maciel Braz                 385618
Francisco Thierry Oliveira Sousa    427340
