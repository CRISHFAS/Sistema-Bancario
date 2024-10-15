# Sistema de Cuenta Bancaria en C

Este programa implementa un sistema de cuenta bancaria básico en C, permitiendo a los usuarios crear cuentas, iniciar sesión, verificar su saldo y transferir dinero entre cuentas. El sistema funciona en la terminal de Windows y utiliza archivos para almacenar datos de usuario y transacciones.

## Características

- **Crear cuenta**: Los usuarios pueden registrarse proporcionando su nombre, detalles personales y tipo de cuenta.
- **Iniciar sesión**: Los usuarios registrados pueden acceder a su cuenta proporcionando su nombre de usuario y contraseña.
- **Consultar saldo**: Una vez iniciado sesión, los usuarios pueden revisar el saldo de su cuenta.
- **Transferencia de dinero**: Los usuarios pueden transferir dinero a otras cuentas registradas.
- **Cerrar sesión**: Los usuarios pueden cerrar sesión y volver al menú principal.

## Funcionalidades Principales

1. **Crear una cuenta**: 
   - Al seleccionar esta opción, el programa solicita información personal y luego crea una cuenta que se guarda en el archivo `username.txt`.
   
2. **Iniciar sesión**: 
   - Los usuarios pueden iniciar sesión proporcionando su nombre de usuario y contraseña. Si el nombre de usuario existe, se les concede acceso a su cuenta.

3. **Transferir dinero**: 
   - Los usuarios pueden transferir dinero a otras cuentas especificando el nombre de usuario del destinatario y el monto a transferir. Esta información se guarda en el archivo `mon.txt`.

4. **Consultar saldo**:
   - Los usuarios pueden ver su historial de transacciones y consultar el saldo total disponible en su cuenta.

5. **Cerrar sesión**:
   - Esta opción permite cerrar la sesión del usuario y regresar al menú principal.

## Estructura de Archivos

El programa utiliza dos archivos principales:

- `username.txt`: Almacena la información de las cuentas de los usuarios.
- `mon.txt`: Almacena los registros de las transferencias de dinero.

## Ejecución

1. **Compilación**:
   Compila el programa usando un compilador compatible con C, como GCC. Si estás en Windows, asegúrate de tener configurado `MinGW` o un entorno similar. Puedes compilarlo con el siguiente comando:

   ```bash
   gcc nombre_del_archivo.c -o sistema_bancario.exe

2. Ejecución: Ejecuta el programa en una terminal de Windows utilizando el siguiente comando:

   ```bash
   sistema_bancario.exe

# Estructura del Código

El programa está organizado de la siguiente manera:

- Estructuras:

- struct pass: Almacena la información del usuario (nombre, fecha de nacimiento, número de teléfono, etc.).
- struct money: Almacena la información de las transferencias de dinero.

### Funciones Principales:

- main(): Muestra el menú principal y gestiona las opciones del usuario.
- account(): Permite crear una nueva cuenta.
- login(): Permite a los usuarios iniciar sesión.
- transfermoney(): Gestiona las transferencias de dinero.
- checkbalance(): Muestra el saldo de la cuenta y las transacciones.
- logout(): Cierra la sesión y regresa al menú principal.

### Requisitos

- Sistema operativo: Windows
- Compilador: Cualquier compilador compatible con C, como GCC.
- Dependencias: windows.h para el uso de funciones de consola específicas de Windows.

## Demostración
Mira el video de demostración [aquí](https://drive.google.com/file/d/1srzIgmaSVf1gpCb-dnEktrioGSAeYKRI/view?usp=sharing).
