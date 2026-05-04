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

# # 🎨 CREACIÓN DE MV Rocky Linux CON SU RESPECTIVA CREACIÓN DE RED PARA LA COMUNICACION CON EL SWITCH Y ROUTER Y LA  ASIGNACIÓN  DE IP ESTATICA:

<img width="1919" height="1037" alt="image" src="https://github.com/user-attachments/assets/e0d55de9-0465-4bf4-ade7-ff857781dc12" />

# Creacion de la IP en Rocky
<img width="660" height="499" alt="Captura de pantalla 2026-04-22 184907" src="https://github.com/user-attachments/assets/f8de615f-b49c-4218-99d2-bd50283ec542" />
<img width="651" height="137" alt="image" src="https://github.com/user-attachments/assets/ccc256e2-0ada-40f3-b607-074b55f81dfb" />

Se observa que la IP queda configurada en Rocky
<img width="657" height="452" alt="image" src="https://github.com/user-attachments/assets/154ffa10-5a97-4e6b-a0a6-0d9f97ad8102" />


# Creación de contendor de Fedora dentro de Rocky Linux 
<img width="679" height="517" alt="image" src="https://github.com/user-attachments/assets/af0d9319-89cd-477a-bf9d-b8fb564085dd" />

Se observa que, aparece root@79f101acddf2, esto indica que nos encontramos dentro de Fedora.

# Nombre del contenedor 
<img width="1899" height="407" alt="image" src="https://github.com/user-attachments/assets/b12e572d-dec3-4cbd-843b-c56ec0487967" />

# Configuración de IP en Fedora:
<img width="1775" height="578" alt="image" src="https://github.com/user-attachments/assets/1e8bcc31-1286-4e37-b935-14737a336f02" />































