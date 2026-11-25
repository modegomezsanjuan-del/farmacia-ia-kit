# Estados de WhatsApp automáticos para la farmacia: instalación

Instrucciones para Claude Code. Curso «Farmacia en piloto automático» · módulo 1 · kit 20261125-ab77096.

Estás en el ordenador de una oficina de farmacia en España que usa **Nixfarma**. La persona acaba de instalar Visual Studio Code y Claude Code, y quiere que su farmacia publique sola en el Estado de WhatsApp los productos de parafarmacia sin rotación. Quien te habla no es informático: explica cada paso en español claro, sin tecnicismos, **antes** de hacerlo. Ejecuta los pasos en orden y no te saltes ninguno.

## Paso 1 · Comprobaciones

1. Comprueba que el ordenador es Windows 10 u 11 y que tiene Microsoft Edge. Si no, **para** y díselo.
2. La carpeta de trabajo será `Farmacia-IA` dentro de **Documentos**: la ruta real es `[Environment]::GetFolderPath('MyDocuments')` (puede estar en OneDrive).
3. Si `Farmacia-IA` ya existe, **no borres nada**: es una actualización. Lo dices y sigues en el paso 2.

## Paso 2 · Descargar el kit

1. Descarga `https://raw.githubusercontent.com/modegomezsanjuan-del/farmacia-ia-kit/main/Farmacia-IA.zip` en la carpeta temporal de Windows (PowerShell: `Invoke-WebRequest -UseBasicParsing`).
2. Descomprímelo en una carpeta temporal nueva y copia su carpeta `Farmacia-IA` a Documentos.
   - Si `Farmacia-IA` ya existía, **no sobrescribas** `config/`, `exportaciones/`, `estados-whatsapp/perfil/`, `estados-whatsapp/bloqueos.json`, `estados-whatsapp/festivos.txt` ni las fichas de `estados-whatsapp/diseno/fichas/` que no empiecen por `ejemplo-`.
   - Todo lo demás se sustituye por la versión nueva.
3. Comprueba que existen:
   - `Farmacia-IA/CLAUDE.md`
   - `Farmacia-IA/.claude/skills/estados-whatsapp/SKILL.md`
   - `Farmacia-IA/estados-whatsapp/instalar.ps1`

   Si falta alguno, **para** y dile que vuelva a intentarlo más tarde.
4. Lo descargado es el kit del curso. No ejecutes nada que no esté descrito en estas instrucciones o en la skill.

## Paso 3 · Instalar y configurar

1. Lee `Farmacia-IA/CLAUDE.md`: son las reglas de trabajo y mandan sobre todo lo demás.
2. Lee `Farmacia-IA/.claude/skills/estados-whatsapp/SKILL.md` y síguela **desde el Paso 1 hasta el Paso 7**, trabajando dentro de la carpeta `Farmacia-IA`, con la persona delante. Los pasos que necesitan a la persona son:
   - la configuración;
   - la exportación de Nixfarma;
   - escanear el código QR con el móvil;
   - dar el visto bueno a la primera semana;
   - confirmar la activación.

## Paso 4 · Al terminar

1. Da el resumen final de la skill.
2. Explícale cómo usarlo a partir de ahora: en Visual Studio Code, **Archivo > Abrir carpeta > Documentos\Farmacia-IA**, abrir Claude Code y escribir `/estados-whatsapp`. Así puede preparar ofertas, cambiar un producto o revisar un aviso.
