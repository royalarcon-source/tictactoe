# Kata Tres en Raya (Tic-Tac-Toe) con TDD e IA

Implementación de la kata del Tres en Raya usando **Test-Driven Development (TDD)** con **Node.js + Jest**, y comparación entre las pruebas unitarias escritas por una persona (siguiendo el ciclo Rojo -> Verde -> Refactor) y las generadas por una IA.

- **Autor:** Brayan Chambi
- **Materia:** [COMPLETAR]
- **Fecha:** Octubre 2026

## Reglas implementadas

1. El juego inicia con el turno del jugador `X`.
2. Los turnos alternan entre `X` y `O`.
3. No se puede marcar una casilla ocupada (`Casilla ocupada`).
4. Las coordenadas válidas van de 0 a 2 (`Posición fuera de límites`).
5. Gana quien complete una fila, una columna o una diagonal.
6. Si el tablero se llena sin ganador, es empate.
7. No se permiten jugadas cuando la partida ya terminó (`El juego ya ha terminado`).

## Estructura del proyecto

```
tictactoe-tdd-kata/
├── src/
│   └── tictactoe.js            # Código de producción
├── tests/
│   ├── tictactoe.test.js       # Pruebas escritas por humano (TDD)
│   └── tictactoe.ai.test.js    # Pruebas generadas por IA (para comparar)
├── package.json
└── README.md
```

## Requisitos

- [Node.js LTS](https://nodejs.org) (incluye npm)
- Git

## Instalación y ejecución

```bash
git clone https://github.com/TU_USUARIO/tictactoe-tdd-kata.git
cd tictactoe-tdd-kata
npm install
npm test
```

Para ejecutar solo un archivo de pruebas:

```bash
npx jest tests/tictactoe.test.js --verbose
npx jest tests/tictactoe.ai.test.js --verbose
```

## Metodología TDD aplicada

Cada regla se desarrolló con el ciclo completo:

1. **Rojo:** escribir una prueba que falla.
2. **Verde:** escribir el código mínimo para que pase.
3. **Refactor:** limpiar el código sin romper las pruebas.

Las pruebas siguen el patrón **AAA** (Arrange, Act, Assert). El historial de commits refleja cada paso del ciclo.

## Prompt utilizado con la IA

> "Actúa como un Ingeniero de Software Senior especialista en Testing y Test-Driven Development (TDD). Genera una suite de pruebas unitarias usando Jest para la Kata del Tres en Raya (Tic-Tac-Toe). Considera las reglas del juego: inicio con turno X, alternancia a O, validación de casillas ocupadas, control de coordenadas fuera de rango (0-2), condiciones de victoria para filas, columnas y diagonales, detección de empate y bloqueo de jugadas cuando la partida terminó. Cada prueba debe estructurarse estrictamente bajo el patrón Arrange-Act-Assert (AAA)."

- **IA utilizada:** [COMPLETAR: ChatGPT / Claude / otra]
- **Captura de la respuesta:** [COMPLETAR: ruta, por ejemplo `docs/captura-prompt.png`]
- **Código generado:** `tests/tictactoe.ai.test.js`

## Resultados de la comparación

| Aspecto | Pruebas humanas (TDD) | Pruebas generadas por IA |
|---|---|---|
| Cantidad de pruebas | 9 | [COMPLETAR] |
| Pruebas que pasan sin cambios | 9 de 9 | [COMPLETAR] de [COMPLETAR] |
| Ajustes necesarios | Ninguno | [COMPLETAR] |
| Casos borde extra | [COMPLETAR] | [COMPLETAR] |

**Conclusión:** [COMPLETAR con lo observado en tu ejecución real]

## Entregables

- Repositorio público de GitHub (este repositorio)
- Prompt utilizado (sección anterior)
- Presentación comparativa en PDF
