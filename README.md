# RAK833-LoRaGateway-RPi

This is a fork of the [RAK833-LoRaGateway-RPi](https://github.com/RAKWireless/RAK833-LoRaGateway-RPi) with updates for the Thing Innovations RAK833 Hat.

Based on the latest SX1301 driver [lora_gateway](https://github.com/Lora-net/lora_gateway) v5.0.1 and semtech [packet_forwarder](https://github.com/Lora-net/packet_forwarder) v4.0.1  

Notes: 

     * This project is only for the SPI interface of RAK833 + Raspberry Pi.
     * The reset GPIO pin definition SX1301_RESET_BCM_PIN macro in the ttnstart.sh file is set to pin 25.

##	Installation procedure

Step 1 : Download and install [Raspbian Stretch LITE](https://www.raspberrypi.org/downloads/raspbian/)

      * Ensure SPI is enabled
      * Serial console is disabled but UART is enabled
      * SSH Enabled

Step 2 : Clone the installer and start the installation

      $ sudo apt-get install git
      $ git clone https://github.com/thiseldo/RAK833-LoRaGateway-RPi.git ~/rak833-loragateway
      $ cd ~/rak833-loragateway
      $ sudo ./install.sh

Step 3 : Now you have a running gateway after restart! in additon you can check the log info at /var/log/syslog.

Step 4 : Register gateway on The Things Network console https://console.thethingsnetwork.org/gateways/register

