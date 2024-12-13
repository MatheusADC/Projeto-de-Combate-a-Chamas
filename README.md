# Projeto de Combate ao Incêndio

## Descrição
O projeto tem como objetivo desenvolver um dispositivo inteligente para a detecção de chamas, integrando diferentes tecnologias para maior eficiência e precisão. O sistema utiliza um sensor infravermelho (IR) para a detecção física das chamas, complementado por uma webcam conectada a uma rede neural convolucional capaz de identificar visualmente imagens de incêndios. Além de enviar alertas pelo WhatsApp para os números cadastrados, o dispositivo é capaz de acionar automaticamente uma bomba de água, ampliando sua funcionalidade em situações de emergência.

## Requisitos
 - Raspberry Pi 5 Model B Anatel - 4GB 
 - Mini Bomba D’água Submersiva 3-6V
 - Módulo Relé 5V 1 Cana
 - Kit Jumpers 20cm x120 Unidades
 - Sensor de Chama Fogo 760 a 1100 nm
 - Case Raspberry Pi 5 Oficial
 - Cabo Micro HDMI 1,50 Metros
 - Cartão de Memória 64GB MicroSd Kingston Classe 10 com Adaptador

## Instalação da biblioteca gpiod pelo shell do Linux
```
sudo apt-get install -y gpiod
```
## Instalação da biblioteca gpiod pelo gerenciador de pacotes do python
```
pip install gpiod
```
## Verificação da instalação da biblioteca gpiod
```
gpiodetect
```
## Verificação da porta ligada ao pino 21 (flame sensor)
```
gpioinfo
```
## Executar programa no terminal
```
sudo python3 main.py
```
<br>

> [!CAUTION]
> O interpretador do python deve estar no diretório /usr/bin/python3

<br>

## Instalação da biblioteca OpenCV
```
sudo apt install python3-opencv
```
## Instalação da biblioteca numpy
```
sudo apt install python3-numpy
```
<br>

> [!CAUTION]
> Para o projeto foi obrigatório utilizar a versão 1.0 (deprecada) do numpy. Para realizar o downgrade:
> 
> **pip3 install "numpy<2"**

<br>

## Preparação para instalação do TensorFlow
```
sudo apt install libatlas-base-dev
```

## Instalação da biblioteca TensorFlow
```
pip3 install tensorflow --break-system-packages
```

## Instalação da biblioteca sklearn
```
pip3 install scikit-learn --break-system-packages
```

## Verificação da detecção da webcam 
```
lsusb
```

## Instalação do Selenium
```
pip3 install selenium --break-system-packages
```

## Instalação da biblioteca PyMongo
```
pip3 install pymongo --break-system-packages
```

## Novas funcionalidades
Com o objetivo de assistir pessoas com deficiência visual e auditiva, pode-se implementar o uso de um Módulo Buzzer Ativo(5V) e de LEDs, respectivamente.
