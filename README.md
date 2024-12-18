# RapiEatsBackend

## Instalación

Sigue estos pasos para configurar el proyecto en tu máquina local:

1. **Clona el repositorio:**
   ```bash
   git clone https://github.com/Awholf/RapidEatsBackend.git
   cd rapieats_backend
## Configuración
1. **Crea un Entorno Virtual**
   ```bash
   python -m venv env
   source env/bin/activate  # En Windows usa `env\Scripts\activate`
2. **Instala Dependencias**
   ```bash
   pip install -r requirements.txt
3. **Crea el archivo .env**
   ```env
   #Ejemplo de archivo .env (para base de datos compartida)
   SECRET_KEY=clave_secreta_de_django_(se_encuentra_en_settings.py)
   DB_NAME=nombre_de_tu_base_de_datos(especialmente en minuscula)
   DB_USER=usuario_especifico
   DB_PASSWORD=contraseña
   DB_HOST=localhost
   DB_PORT=3306
   DEBUG=True
4. **Aplica migraciones**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
5. **Inicia el sevidor**
   ```bash
   python manage.py runserver
