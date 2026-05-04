# LABORATORIO_2
ALEXANDER REINA-BRAYAN IVAN RIBON QUINTERO-EDWAR ROBERTO MARTINEZ PINTO- LINA MARCELA CONTRERAS SANABRIA-JEIMMI LORENA NIÑO CORREA

# 🔧 Configuración del Router y Switch de la tecnologia Cisco:

<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/1fc2e246-3e40-4fb7-93d0-e0af6638c998" />

<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/39c48e00-3b16-4426-8511-ad6cbcda0590" />

<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/46ccea0a-e3aa-4862-b31c-953184e79c16" />

# 📄 Configuración de Switch Cisco:
Configuración inicial del switch:

<img width="818" height="851" alt="image" src="https://github.com/user-attachments/assets/0a4005ef-c7cb-40ce-b1f4-510799eb465c" />

Creación de VLAN´s y asignación en modo acceso, a su vez la configuración de el protocolo Spanning-tree port fast:

<img width="375" height="183" alt="image" src="https://github.com/user-attachments/assets/080518a1-d92a-428b-aa0b-82e66e0d52f7" />

<img width="772" height="501" alt="image" src="https://github.com/user-attachments/assets/14c392b6-eaeb-4f1a-ab84-d0d3696a64e6" />

# 🔧 configuración establecida en el switch:

<img width="830" height="252" alt="image" src="https://github.com/user-attachments/assets/8c485e5a-4199-4589-8f90-efae1b2793f8" />

# 🔧 configuración de los puertos troncales en el Switch:

<img width="663" height="534" alt="image" src="https://github.com/user-attachments/assets/b555d285-aaa4-47ae-bd60-8330aca91ff6" />

# 🔧 Activación y asignación de subinterfaces desde el Router para la comunicación con las Vlan´s configuradas previamente en el Switch, por último se realiza el encapsulamiento dot1Q con su respectiva IP asiganada a cada Vlan:

<img width="928" height="287" alt="image" src="https://github.com/user-attachments/assets/9c9aa189-e166-4308-8bb3-089fc2287d21" />


<img width="641" height="141" alt="image" src="https://github.com/user-attachments/assets/39b466ef-4d10-4980-bfcd-874750f73b0f" />

# 🎨 CREACIÓN DE CONTENEDOR ALPINE CON SU RESPECTIVA CREACIÓN DE RED PARA LA COMUNICACION CON EL SWITCH Y ROUTER Y LA  ASIGNACIÓN  DE IP ESTATICA:

<img width="812" height="651" alt="image" src="https://github.com/user-attachments/assets/f96d74ab-f367-4521-b66a-19cd323b74e2" />

Asignacion de ip add y iputils para alpine:

<img width="535" height="108" alt="image" src="https://github.com/user-attachments/assets/76d7bd5e-b93d-4a99-a5aa-d701c504aebb" />

<img width="682" height="265" alt="image" src="https://github.com/user-attachments/assets/67d421ae-3ba2-4b9c-9d72-2d38d7907882" />

# 🔧 Se procede a actulizar el contenedor

<img width="678" height="358" alt="Captura desde 2026-04-22 19-51-09" src="https://github.com/user-attachments/assets/e7e707fd-842e-4f90-a1d8-df4047680a63" />

# 🔧 Se realizara la creación de la red para la comunicacion con los demás contenedores y maquinas virtuales:


<img width="985" height="52" alt="Captura desde 2026-05-02 22-57-14" src="https://github.com/user-attachments/assets/67e4f7d8-d688-4634-8e3c-353682812f3b" />


# 🔧 Se valida la creación de la red para este caso es la red red_universidad:

<img width="407" height="244" alt="Captura desde 2026-04-29 18-49-38" src="https://github.com/user-attachments/assets/d4b27f35-d552-4e5c-ac0a-20336e7e119c" />


# 🔧 Luego se realiza la asignación de la IP estatica (192.168.10.8) para el contenedor con su respectiva red previamente creada:

<img width="884" height="72" alt="Captura desde 2026-04-29 18-47-04" src="https://github.com/user-attachments/assets/ae5f42c1-3f4b-4b89-a278-d6765285d3bc" />

# 🔧 Se realiza un reinicio del contenedor para que la asignación de la IP y la red quede correctamente establecida, podemos observara que ya se encuentra establecida la red en la interfaz Eth0:

<img width="370" height="112" alt="Captura desde 2026-04-29 18-47-32" src="https://github.com/user-attachments/assets/fe14eb52-01af-4f44-8efd-cce84c96965e" />


<img width="874" height="628" alt="Captura desde 2026-04-29 18-50-05" src="https://github.com/user-attachments/assets/198edfa7-975c-48eb-be11-f7223fde6463" />

# 📄 NOTA: Ya que el sistema operativo Kali Linux se obtiene de raiz desde un portatil no se realizo virtualización de dicho OS, se demostrara la asignacion de una IP estatica con su respectivo ID red y mascara de red:

KALI LINUX:
<img width="1364" height="760" alt="Captura desde 2026-05-02 23-02-20" src="https://github.com/user-attachments/assets/7295cb17-8166-4929-ba6f-fc07b97880fb" />


<img width="1364" height="767" alt="Captura desde 2026-05-02 23-02-44" src="https://github.com/user-attachments/assets/1cdde3dd-9f2e-4fa0-99b7-7097d0cb81ad" />

# 🔧 Se ingresa al bash de nano y se realiza las siguiente configura, luego con control+o se guarda dicha configuración y con control + x salimos del bash de nano:

<img width="851" height="342" alt="Captura desde 2026-04-29 19-12-20" src="https://github.com/user-attachments/assets/c6cf3120-c9a0-4507-bb3d-7113e71ee497" />

# 🔧 Una vez ya realizado la configuración en nano, ahora se ejecuta un apagado y encendido de la interfaz eth0 para que tome dicha IP estatica (192.165.10.15) al puerto:

<img width="865" height="234" alt="Captura desde 2026-04-29 19-12-41" src="https://github.com/user-attachments/assets/f4f000aa-88e5-47ae-a9f3-5963c7bd90d1" />

# 🔧 Por último ya se observa con el comando ifconfig la comfiguración asignada correctamente:

<img width="613" height="172" alt="Captura desde 2026-04-29 19-12-57" src="https://github.com/user-attachments/assets/9e850057-a67e-4dd8-8009-b9bef587b9fa" />



# Instalacion Servidor Debian LAB2

Esta guia cubre la instalacion y configuracion basica del servidor Debian para el laboratorio 2. Sigue los pasos en orden para evitar errores de dependencias.

---

## Paso 1: Instalar MariaDB

Esto tarda aproximadamente 3 minutos. MariaDB es la base de datos que van a necesitar tanto Zabbix como pmacct, asi que es lo primero que hay que dejar listo.

```bash
sudo apt install -y mariadb-server
```
<img width="801" height="140" alt="image" src="https://github.com/user-attachments/assets/671ff53a-80d4-4716-9364-de64df226c20" />


---

## Paso 2: Instalar Zabbix

### 2.1 Descargar el paquete de release

```bash
wget -q https://repo.zabbix.com/zabbix/6.4/debian/pool/main/z/zabbix-release/zabbix-release_6.4-1+debian12_all.deb
```
<img width="887" height="132" alt="image" src="https://github.com/user-attachments/assets/6592dc4e-cecd-48f3-9180-ffaefb798c62" />


### 2.2 Instalar el paquete de release

```bash
sudo dpkg -i zabbix-release_6.4-1+debian12_all.deb
```

### 2.3 Actualizar indices 

```bash
sudo apt update
```

### 2.4 Instalar Zabbix completo

> **Nota sobre errores de firma GPG:** En Debian 13 es comun que aparezcan errores de firma GPG en el repositorio de Zabbix. La solucion es saltarse la verificacion y usar lo que esta disponible en los repositorios oficiales.

```bash
sudo apt update --allow-insecure-repositories --allow-unauthenticated && sudo apt upgrade -y
```
<img width="858" height="213" alt="image" src="https://github.com/user-attachments/assets/8bbb5bd4-0928-4b7a-9db1-2182619582ed" />

<img width="830" height="372" alt="image" src="https://github.com/user-attachments/assets/7ac075c0-1e33-4004-947a-5c01c0834b03" />


```bash
sudo apt install -y --allow-unauthenticated zabbix-apache-conf zabbix-sql-scripts
```

### 2.5 Instalar todos los componentes de Zabbix

```bash
sudo apt install -y zabbix-server-mysql zabbix-frontend-php zabbix-apache-conf \
    zabbix-sql-scripts zabbix-agent mariadb-server
```
<img width="826" height="403" alt="image" src="https://github.com/user-attachments/assets/4d940fdb-9ff6-4632-a44e-d48f2cb6545c" />


### 2.6 Configurar la base de datos

Esto crea la base de datos de Zabbix y el usuario con sus permisos. Ejecuten el bloque completo de una vez:

```bash
sudo mysql -u root << 'EOF'
DROP DATABASE IF EXISTS zabbix;
DROP USER IF EXISTS 'zabbix'@'localhost';
CREATE DATABASE zabbix CHARACTER SET utf8mb4 COLLATE utf8mb4_bin;
CREATE USER 'zabbix'@'localhost' IDENTIFIED BY 'zabbixpass';
GRANT ALL PRIVILEGES ON zabbix.* TO 'zabbix'@'localhost';
FLUSH PRIVILEGES;
EXIT;
EOF
```
<img width="763" height="385" alt="image" src="https://github.com/user-attachments/assets/444e3d0f-7ddf-4fc9-a755-39c1b44d3e8b" />


### 2.7 Importar el esquema de la base de datos

```bash
zcat /usr/share/zabbix-sql-scripts/mysql/server.sql.gz | mysql -u zabbix -pzabbixpass zabbix
```

### 2.8 Editar el archivo de configuracion de Zabbix

```bash
sudo nano /etc/zabbix/zabbix_server.conf
```

Busquen las siguientes lineas y dejelas asi (o agrefuenlas si no estan):

```
DBName=zabbix
DBUser=zabbix
DBPassword=zabbixpass
```

Guardar con `Ctrl+O` -> `Enter` -> `Ctrl+X`

### 2.9 Habilitar y reiniciar los servicios

```bash
sudo systemctl restart zabbix-server-mysql zabbix-agent grafana-server apache2
sudo systemctl enable zabbix-server-mysql zabbix-agent grafana-server apache2
```

---

## Paso 3: Configurar VLANs y herramientas de red

Esta parte configura las VLANs del servidor. Tarda aproximadamente 5 minutos.

### 3.1 Cargar el modulo 8021q

```bash
sudo modprobe 8021q
echo "8021q" | sudo tee -a /etc/modules
```
<img width="913" height="163" alt="image" src="https://github.com/user-attachments/assets/b6960dd4-8929-449f-ba78-768e157aebc2" />


### 3.2 Habilitar IP Forwarding

```bash
sudo sysctl -w net.ipv4.ip_forward=1
echo "net.ipv4.ip_forward=1" | sudo tee -a /etc/sysctl.conf
```
<img width="842" height="82" alt="image" src="https://github.com/user-attachments/assets/8a46256d-3392-43da-95bf-7a16d6252c9e" />


### 3.3 Crear las interfaces VLAN

```bash
sudo ip link set enp0s8 up
sudo ip link add link enp0s8 name enp0s8.10 type vlan id 10
sudo ip link add link enp0s8 name enp0s8.20 type vlan id 20
sudo ip link set enp0s8.10 up
sudo ip link set enp0s8.20 up
```
<img width="896" height="107" alt="image" src="https://github.com/user-attachments/assets/06151d86-a7ae-40fc-b06e-d8cd04856c2d" />


### 3.4 Asignar IPs a las VLANs

```bash
sudo ip addr add 192.168.10.1/24 dev enp0s8.10
sudo ip addr add 192.168.20.1/24 dev enp0s8.20
```
<img width="792" height="72" alt="image" src="https://github.com/user-attachments/assets/ea35004f-fe76-409f-95c7-91d09b97c592" />


### 3.5 Verificar que quedo bien

```bash
ip addr show enp0s8.10
ip addr show enp0s8.20
ip route show
```

La salida deberia mostrar algo asi:

```
inet 192.168.10.1/24
inet 192.168.20.1/24
```
<img width="826" height="456" alt="image" src="https://github.com/user-attachments/assets/59927b58-19a1-4a65-b50c-827f0eecc6ab" />

### 3.6 Hacer la configuracion permanente (sobrevive reinicios)

Abran el archivo de interfaces:

```bash
sudo nano /etc/network/interfaces
```

Agregen esto al final del archivo:

```
auto enp0s3
iface enp0s3 inet manual
    up ifconfig $IFACE 0.0.0.0 up

auto enp0s3.10
iface enp0s3.10 inet static
    address 192.168.10.1
    netmask 255.255.255.0
    vlan-raw-device enp0s3

auto enp0s3.20
iface enp0s3.20 inet static
    address 192.168.20.1
    netmask 255.255.255.0
    vlan-raw-device enp0s3
```

Guardar con `Ctrl+O` -> `Enter` -> `Ctrl+X`

### 3.7 Reiniciar la red

```bash
sudo systemctl restart networking
```

### 3.8 Verificacion final

```bash
ip addr show | grep -E "enp0s3|inet"
```

---

## Paso 4: Verificar que Grafana este corriendo

```bash
sudo systemctl status grafana-server
```

Si todo salio bien, deberia aparecer:

```
Active: active (running)
```
<img width="907" height="495" alt="image" src="https://github.com/user-attachments/assets/21a4f730-6800-4cda-afbe-dd89c403e83a" />

#  CREACIÓN DE MV Rocky Linux CON SU RESPECTIVA CREACIÓN DE RED PARA LA COMUNICACIÓN CON EL SWITCH Y ROUTER Y LA ASIGNACIÓN DE IP ESTATICA:
<img width="1919" height="1037" alt="image" src="https://github.com/user-attachments/assets/f867eb8a-0558-4cff-b158-b443b7fc8223" />

# Creacion de la IP en Rocky
<img width="660" height="499" alt="image" src="https://github.com/user-attachments/assets/decb9184-70b9-4d1a-acbd-413e94afb855" />
<img width="651" height="137" alt="image" src="https://github.com/user-attachments/assets/1f94ea4c-2a1b-48c6-800c-378810560a9d" />

Se observa que la IP queda configurada en Rocky

<img width="657" height="452" alt="image" src="https://github.com/user-attachments/assets/3d589757-e55f-4cf4-8284-999abe044c40" />

# Creación del contendor de Fedora dentro de Rocky Linux 
<img width="679" height="517" alt="image" src="https://github.com/user-attachments/assets/9f2423cf-d80e-4f7d-ac80-b89c37e8a647" />

Se observa que, aparece root@79f101acddf2, esto indica que nos encontramos dentro de Fedora.

# Nombre del contenedor 
<img width="1899" height="407" alt="image" src="https://github.com/user-attachments/assets/ca9818b1-9e26-48e9-b164-5146289b308a" />

# Configuración de IP en Fedora:
<img width="1775" height="578" alt="image" src="https://github.com/user-attachments/assets/f5beea40-f756-4ed7-92f9-7cab9f7128b9" />






























