# Windscribe

### Instrucciones para distribuciones basadas en **Debian/Ubuntu**:

1. **Actualiza los repositorios e instala los paquetes necesarios**:

   ```bash
   sudo apt update
   sudo apt install apt-transport-https curl
   ```

2. **Importa la clave GPG de Windscribe**:

   ```bash
   curl -fsSL https://repo.windscribe.com/ubuntu/key.gpg | sudo tee /etc/apt/trusted.gpg.d/windscribe.gpg > /dev/null
   ```

3. **Añade el repositorio de Windscribe**:

   ```bash
   echo "deb https://repo.windscribe.com/ubuntu bionic main" | sudo tee /etc/apt/sources.list.d/windscribe-repo.list
   ```

   Nota: Aunque `bionic` está en el comando, es compatible con versiones recientes de Ubuntu y Debian.

4. **Instala Windscribe**:

   ```bash
   sudo apt update
   sudo apt install windscribe-cli
   ```

5. **Inicia sesión en Windscribe** (Usa tus credenciales de Windscribe):

   ```bash
   windscribe login
   ```

6. **Conéctate a un servidor** (puedes usar `best` para conectarte al mejor servidor disponible):

   ```bash
   windscribe connect
   ```

   O elige una ubicación específica:

   ```bash
   windscribe connect [ubicación]
   ```

7. **Verifica el estado de la conexión**:

   ```bash
   windscribe status
   ```

8. **Para desconectarte**:

   ```bash
   windscribe disconnect
   ```

