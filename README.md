1. Aplicaciones necesarias e instalaciónVisual Studio Code: Editor de código principal.Node.js (versión LTS): Descargar desde nodejs.org si no está instalado. Incluye npm.Git: Para gestionar el repositorio local y sincronizarlo con GitHub.   PowerPoint, Google Slides o Canva: Para armar y exportar la presentación a PDF.   2. Configuración del proyecto paso a pasoAbre tu terminal (PowerShell o Git Bash) y ejecuta los siguientes comandos:Bash# 1. Crear y entrar a la carpeta del proyecto
mkdir tictactoe-tdd-kata
cd tictactoe-tdd-kata

# 2. Inicializar proyecto Node.js
npm init -y

# 3. Instalar Jest (framework de pruebas unitarias)
npm install --save-dev jest

# 4. Crear carpetas de código y pruebas
mkdir src tests
Modifica el archivo package.json para que el script test use Jest:JSON"scripts": {
  "test": "jest --verbose"
}


