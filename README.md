# kernel-tunning

Configurações para kernel
## Lista de configurações:

### Sysfs
 - cpu-conservative.conf (/etc/sysfs.d/cpu-conservative.conf)

### Para adicionar módulos ao initramfs:
Primeiro abra o arquivo de módulos do initramfs:

```sh
nano /etc/initramfs-tools/modules
```

Depois coloque a linha de um módulo que deseja carregar (por exemplo cpufreq_conservative)

feche e execute o comando para a atualização do initramfs para todos os kernels da máquina:

```sh
sudo update-initramfs -u -k all
```
