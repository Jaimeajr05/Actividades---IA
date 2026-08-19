# Actividad de Clase: Analizando Agentes de IA con Hugging Face Spaces

## Objetivo

Explorar aplicaciones reales de Inteligencia Artificial en **Hugging
Face Spaces** y analizarlas desde la perspectiva de los **agentes
racionales**.

Al finalizar la actividad, los estudiantes deberán ser capaces de:

-   Identificar los componentes **PEAS** de un agente.
-   Clasificar las propiedades del entorno.
-   Proponer qué tipo de programa de agente podría implementarse detrás
    del sistema.
-   Justificar sus respuestas.

------------------------------------------------------------------------

## Instrucciones

1.  Ingresen a **https://huggingface.co/spaces**.
2.  Exploren diferentes Spaces.
3.  Seleccionen uno que les parezca interesante.
4.  Interactúen con el sistema durante algunos minutos.
5.  Completen la siguiente ficha de análisis.

------------------------------------------------------------------------

# Ficha de análisis

## 1. Nombre del Space

**Nombre:mrfakename/Z-Image-Turbo**

**Enlace: https://huggingface.co/spaces/mrfakename/Z-Image-Turbo**

------------------------------------------------------------------------

## 2. ¿Qué hace el agente?

Describa en dos o tres líneas cuál es la función del sistema.

Es un agente que genera imagen a partir de texto. Ademas de generar una semilla para poder replicar la misma imagen. 

------------------------------------------------------------------------

## 3. Análisis PEAS

  Elemento          Respuesta
  ----------------- ----------------------------------------------------
  **Performance**   ¿Qué significa que el agente haga bien su trabajo?
                    Que la imagen cumpla con lo propuestos en el texto o desde objetivos como estetica, realismo, etc.  
  **Environment**   ¿Con qué interactúa el agente?
                    Desde la creacion de la imagen y ver como evoluciona desde las iteraciones que pueda tener la misma, ademas del texto que pone el usuario para                     generar la imagen. 
  **Actuators**     ¿Qué acciones produce?
                    Los pixeles dados para representar la imagen 
  **Sensors**       ¿Qué información recibe como entrada?
                    El espacio de texto dado para el usuario y visualizacion de las imagenes iteradas.

------------------------------------------------------------------------

## 4. Clasificación del entorno

Complete la siguiente tabla y justifique brevemente cada respuesta.

  Propiedad      Clasificación     Justificación
  -------------- ----------------- ---------------
  Observable     Total             Dado que siempre tiene la informacion completa con la que trabaja, en este caso la dada por el usuario 
  Determinista   No                Puede cambiar cada vez que uno genera una imagen por eso se da una semilla 
  Episódico      No                Dado que es directa la imagen con el texto dado
  Estático       Sí                No cambia de estado despus de generar la imagen.
  Discreto       Sí                Es una imagen, un numero de cacateres
  Conocido       No aplica         No Existe leyes fisicas, es un entono vitual 

------------------------------------------------------------------------

## 5. ¿Qué tipo de programa de agente creen que es?

Seleccione la opción que consideren más adecuada y explique por qué.

-   Agente de reflejo simple
-   Agente basado en modelo 
-   Agente basado en objetivos
-   Agente basado en utilidad
-   Agente con aprendizaje

> **Importante:** No existe una única respuesta correcta. Lo importante
> es justificar la elección a partir del comportamiento observado.

------------------------------------------------------------------------

Diria que es un Agente basado en modelo dado que su objetivo es generar una imagen dada el texto del usuario que se verifica en cada iteracion de creacion de imagen 

# Discusión en clase

Después de las presentaciones, discutiremos preguntas como:

-   ¿Dos Spaces diferentes pueden compartir el mismo tipo de entorno?
    No crearia. 
-   ¿Es posible saber con certeza qué tipo de agente implementa un Space
    únicamente observándolo?
    No, se debe saber como este funciona internamente para poder entenderlo en completitud 
-   ¿Qué diferencia existe entre el comportamiento observable de un
    agente y su implementación interna?
    El comportamiento obserbalble radica mas en el resultado final del agente y su implementacion interna muestra todas la tranformaciones que tuvo la entrada         hasta el resultado final. 

------------------------------------------------------------------------

# Reto adicional

Encuentre un Space que pueda clasificarse como:

1.  **Totalmente observable, determinista y episódico.**
    Omni Editor 2.0  
   
3.  **Parcialmente observable, estocástico y secuencial.**
    victor/gemma-avatar

Justifique su respuesta.

------------------------------------------------------------------------

# Rúbrica (10 puntos)

| Criterio | Puntos |
|-----------|:------:|
| Descripción correcta del Space | 2 |
| Identificación de PEAS | 3 |
| Clasificación del entorno | 3 |
| Justificación del tipo de agente | 2 |
| **Total** | **10** |

------------------------------------------------------------------------


