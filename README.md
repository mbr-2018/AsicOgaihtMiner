Asic OgaihtMiner

A Asic OgaihtMiner é uma máquina de mineração de Bitcoin DESENVOLVIDA EXCLUSIVAMENTE NO BRASIL, ainda em fase experimental e estágio inicial. Equipado com um único ASIC Bitmain BM1397AD, oferece uma solução inovadora para mineradores que buscam eficiência e desempenho em um produto nacional.


Estado Atual

- Projeto em fase de PROTÓTIPO.
- Em breve, a PCB estará disponível para testes e produção.

Software OS

- Em desenvolvimento.
- O firmware conectará o dispositivo a pools de mineração via Wi-Fi e fará o gerenciamento completo do ASIC.



Conexões BM1397AD

| Nome do Pino | Descrição |
|--------------|-----------|
| VIN          | Alimentação do núcleo do ASIC (aproximadamente 1.0 á 1.62V.) |
| +5V          | Entrada de 5V (regulada para 1.8V e 0.8V); também alimenta o fan. Opcional se ESP32 estiver via USB |
| +5V (Fan)    | Saída de 5V para a ventoinha |
| SPD (Fan)    | Entrada de sinal de velocidade da ventoinha |
| VIO          | Tensão dos GPIOs do ESP32-C3 (3.3V) |
| RXI          | Entrada serial (nível 1.8V) |
| TXO          | Saída serial (nível 1.8V) |
| RST          | Sinal de reset invertido para o BM1397AL |
| GND          | Terra comum |

- O BM1397AD é um chip ASIC SHA256 da Bitmain, amplamente utilizado no Antminer S17,.
- Possui hashrate de até 400 á 453GH/s e uma eficiência de 0,03 J/GH. ( Confomre Descrição da Bitmain)
- Fisicamente similar ao BM1387, mas com pinagem diferente.

Objetivos

- Desenvolver firmware para ESP32-C3 com:
- Conexão Wi-Fi com servidores Stratum/pools
- Monitoramento da ventoinha
- Leitura de temperatura via NCT218
- Criar software em **Rust** para:
- Obter blocos via nó Bitcoin
- Distribuir trabalho para dispositivos OgaihtMiner
- Adicionar sensor de consumo elétrico para controle dinâmico de frequência e corrente (ideal para setups com energia solar)


*Eficiência e inovação para quem busca liberdade na mineração.*

