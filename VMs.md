# Hyper-v
## Ubuntu 20.04
### Evitar lag en pantalla: 
1. Run:
```console
 sudo nano /etc/modprobe.d/blacklist.conf
```
2. Add the following line at the end of the file:
```console
blacklist hyperv_fb
```
3. Save (Ctrl+X then Y)
4. Reboot
```console
sudo reboot
```
### Aumentar resolucion
1. abrir powershell como administrador en el host
2. colocar el siguiente codigo:
```console
 set-vmvideo -vmname NOMBREDETUVM -horizontalresolution:1920  -verticalresolution:1080 -resolutiontype single
```
Escoger la resolucion correspondiente
