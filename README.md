# Inatalando - Go, GRPC y Protocol Buffer

**Tested** On:
    1. Ubuntu 18.04 
    2. Ubuntu 20.04 

## Instalación
#### Instalar git

```
sudo apt update 
sudo apt install git -y
```

#### Ejecute las siguientes líneas 
```sh
git clone https://github.com/amb1s1/grpc-proto-buffer-install.git ~/
cd ~/grpc-proto-buffer-install
```

##### Installar go
```sh
./go_install.sh
```

#### Pegue esto en el shell o edite su archivo bashrc
##### Go y gRPC necesitan estos paths
```
export GOPATH=$HOME/gocode
export PATH=/usr/local/go/bin:$HOME/grpc/bins/opt/:$HOME/bin:/usr/local/bin:$GOPATH/bin:$PATH
```
#### Ejecute las siguientes líneas 
##### Installar grpc y protoc

```
./grpc_proto_install.sh
```

### Prueba tu instalación
#### Obtén el código de ejemplo
*El código de ejemplo es parte del repositorio grpc-go.*

##### Descargue el repositorio como un archivo zip y descomprímalo, o clone el repositorio:

```sh
git clone -b v1.35.0 https://github.com/grpc/grpc-go ~/
```

##### Cambiar al directorio de ejemplo de inicio rápido

```
cd ~/grpc-go/examples/helloworld
```

#### Ejecuta el ejemplo

*Desde el directorio examples/helloworld:*

*Compile y ejecute el código del servidor:*

```
go run greeter_server/main.go
```

*Desde una terminal diferente, compile y 
ejecute el código del cliente para ver 
la salida del cliente:*

```
go run greeter_client/main.go
```

*Si todo trabaja bien, debes de recivir este mensaje:*

```
        Greeting: Hello world
```

¡Felicidades! Acaba de ejecutar una aplicación cliente-servidor con gRPC.


