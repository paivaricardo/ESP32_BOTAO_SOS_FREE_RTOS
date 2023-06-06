# ESP32_BOTAO_SOS_FREE_RTOS

Repositório para armazenar uma implementação de um botão de SOS em um sistema embarcado, com uso do sistema FreeRTOS e a placa ESP32, com conectividade à Internet por meio da placa DOIT ESP32 DEVKIT V1, utilizando um broker MQTT.

Projeto apresentado como trabalho final da disciplina Sistemas em Tempo Real e Embarcados do curso de Ciência da Computação do Centro Universitário de Brasília (CEUB).

Placa microcontroladora utilizada no projeto: DOIT ESP32 DEVKIT V1 (WiFi).

## Configurando a Arduino IDE
Link para o pacote para a instalação da placa microcontoladora na Arduino IDE (acrescentar a seguinte URL no menu Preferências -> Aditional Board Manager URLs da Arduino IDE):
https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json 

Após isso, selecione como placa "DOIT ESP32 DEVKIT V1" para seu projeto.

## Acrescentando as credenciais para conexão WiFi e acesso ao servidor MQTT
Para utilizar a aplição, é necessário criar os headers para acrescentar as credenciais para a conexão WiFi e acesso ao servidor MQTT. Para isso, há dois templates neste repositório.

### Credenciais WiFi
Copie o arquivo WiFiCredentials_Template.h e renomeie como WiFiCredentials.h. Defina as seguintes variáveis no arquivo:
- SSID: <<SSID da rede WiFi à qual a placa ESP32 vai se conectar>>
- PASSWORD: <<Senha da rede WiFi à qual a placa ESP32 vai se conectar>>

### Credenciais MQTT
Copie o arquivo MQTTCredentials_Template.h e renomeie como MQTTCredentials.h. Defina as seguintes variáveis no arquivo:
- BROKER_MQTT: <<URL do broker MQTT ao qual serão enviadas mensagens>>
- BROKER_PORT: <<Porta do broker MQTT à qual serão enviadas mensagens>>