# Algorithmic Trading Battle Simulator

Competencia animada entre estrategias de trading sobre el **SPY (2018–2023)** con backtesting.

## Estrategias

- **Momentum:** cruce de medias móviles (20/50).
- **Mean Reversion:** RSI (14) con umbrales 30/70.
- **Random:** referencia aleatoria.

## Qué hace

- Backtesting con señales desplazadas un día para no usar información futura.
- Curva de capital de cada estrategia y animación tipo carrera con marcador y líder.
- Métricas: retorno acumulado, Sharpe, máximo drawdown y win rate.

## Estructura

- `main.py` — datos, backtesting y animación
- `strategies.py` — estrategias
- `backtester.py` — motor de backtesting y métricas

## Cómo ejecutarlo

```bash
pip install -r requirements.txt
python main.py
```

## Limitaciones

- **Mejora pendiente:** el Sharpe y el win rate se calculan sobre los retornos del SPY y no sobre los de cada estrategia, por eso salen iguales en las tres.
- Sin costos de transacción y con parámetros fijos.

## Autor

**Santiago Peña Díaz** — Estudiante de Ingeniería de Sistemas (CUN, Colombia)

- GitHub: [Lmao320](https://github.com/Lmao320)
- Documentación completa: [Portafolio en Notion](https://freezing-hope-5b5.notion.site/Portafolio-de-Proyectos-Santiago-Pe-a-D-az-41f7f18e4ca2811793dcece91c3d00c0)
