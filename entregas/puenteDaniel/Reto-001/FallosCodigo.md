# Analisis Legibilidad

## 1.Nombres descripctivos
| Archivo      |    Linea     |    Recomendacion / Problema |
|--------------|--------------|------------------|
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java#) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L20) |Nombre genérico para una coordenada específica. Mejor coordenada  |
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java#) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L4) |  Nombre de clase poco descriptivo. No revela que es un juego de rescate de soldados. |
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L39) | Nombres genéricos que no indican su propósito en el contexto |


## 2.Lógica Estructural Incorrecta
| Archivo      |    Linea     |    Recomendacion / Problema |
|--------------|--------------|------------------|
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L28) |  El método inicializarJuego() contiene dos responsabilidades distintas: inicializar tablero y colocar soldados. |
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L74) | Validación de coordenadas que debería ir antes de la conversión para evitar excepciones potenciales.  |

## 3.Convenciones de Java Incumplidas
| Archivo      |    Linea     |    Recomendacion / Problema  |
|--------------|--------------|------------------|
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L12) | Método main() con mucho código en lugar de delegar a otros métodos.  |
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L77) | Condición compleja con múltiples operaciones lógicas que dificulta la lectura.  |

## 4. Errores de Semántica
| Archivo      |    Linea     |    Recomendacion / Problema |
|--------------|--------------|------------------|
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L70) | No se decrementa el contador de turnos cuando se ingresa una coordenada inválida.  |
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L75) |  No se maneja correctamente la posibilidad de que la entrada tenga un formato incorrecto.  |

# 5.Código DRY
| Archivo      |    Linea     |    Recomendacion / Problema |
|--------------|--------------|------------------|
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L52) | Código repetitivo para mostrar el tablero que podría refactorizarse..  |
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L64) |   Información repetitiva en la salida del programa.  |

# 6.Falta de Modularidad y Cohesión
| Archivo      |    Linea     |    Recomendacion / Problema |
|--------------|--------------|------------------|
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L13) | El método main() hace demasiadas cosas directamente.  |
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L68) | El método procesarEntrada() combina validación, conversión y lógica de juego.  |
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L50) | El método mostrarTablero() tiene demasiada responsabilidad.  |

# 7.Nombres de Variables Confuso
| Archivo      |    Linea     |    Recomendacion / Problema |
|--------------|--------------|------------------|
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L73) | Conversión de coordenadas fila y columna confusa y propensa a errores. |
| [Rescate](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/main/src/Rescate.java) | [Ver](https://github.com/Ingenieria-Informatica-UNEATLANTICO/23-24-prg1-examen-final-danielpuentesaranana/blob/c470a8180c8285049081699eb03e17946529ab02/src/Rescate.java#L5) |Variables estáticas de clase que deberían tener nombres más descriptivos.  |



# 8. Falta de Comentarios Explicativos


- Falta explicación de las reglas del juego y la lógica detrás del rescate.
  
- No hay comentarios que expliquen la representación visual de los soldados (" \\O/" en línea 55).

- No hay separación clara entre modelo, vista y controlador.
