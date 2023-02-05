## Tema 4 - Redes en Docker

### Parte 1- Trabajar con redes docker

1. Vamos a crear dos redes de ese tipo (BRIDGE) con los siguientes datos:
 - Red1: Nombre: red1; Dirección de red: 172.28.0.0; Máscara de red: 255.255.0.0; Gateway: 172.28.0.1

- Red2: Nombre: red2. El resto de los datos será proporcionados automáticamente por Docker.

Creamos la red1

```bash
docker network create -d bridge red1 --subnet 172.28.0.0/16 --gateway 172.28.0.1
```

La ip es /16 debido a que su máscara de red.


Creamos la red2:

```bash
docker network create -d bridge red2
```

![](assets/ejercicio1.png)

![](assets/ejercicio1-red1.png)

![](assets/ejercicio1-red2.png)



