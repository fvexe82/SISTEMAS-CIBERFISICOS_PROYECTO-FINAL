# Carpeta que contiene los componentes, archivos y requisitos necesarios para la simulación.
# Elementos a tener en cuenta en la simulación
![pcsimucip](https://github.com/fvexe82/SISTEMAS-CIBERFISICOS_PROYECTO-FINAL/assets/106171748/6d4ed491-07d5-47b9-a5f7-126652091d3a)

## Componentes:

  * Pilotos LED: H1, H2, H3
  * Pulsadores: Rt, PG, PM
  * Bombas: M1 (carga), M2 (envío)
  * Válvulas: V1 (entrada de soda cáustica), V2 (entrada de agua caliente), V3 (entrada de agua fría), V4 (salida/vaciado general)
  * Sensores de Nivel: B2 (nivel mínimo), B1 (nivel máximo)

## Tareas:
Fase de Soda Cáustica:
  * Al presionar PM, M1 se activa y V1 se abre para llenar el tanque de soda cáustica.
  * H1 se enciende en verde mientras el tanque se está llenando con soda cáustica.
  * Una vez alcanzado el nivel deseado, V1 se cierra.

Fase de Agua Caliente:
  * Con M1 aún en funcionamiento, V2 se abre para llenar el tanque de agua caliente.
  * H2 se enciende en verde mientras el tanque se está llenando con agua caliente.
  * Tras alcanzar el nivel deseado, V2 se cierra.

Fase de Agua Fría:
  * M1 sigue funcionando y V3 se abre para llenar el tanque con agua fría.
  * H1 y H2 se apagan, y H3 se enciende en verde durante esta fase.
  * Una vez alcanzado el nivel deseado, V3 se cierra.

Selección del Tanque para CIP:
  * Luego de la preparación, se activará la bomba M2 que seleccionará el tanque adecuado para comenzar con el proceso CIP en la maquinaria y
procesos correspondientes.

Vaciado y Finalización:
  * V4 se abrirá para vaciar completamente los tanques si es necesario.

Una vez vaciado, todos los pilotos se apagan indicando la finalización del proceso.

PG es una parada de emergencia. Al presionarse, todo el proceso debe
detenerse inmediatamente. H3 se encenderá en rojo cuando se active la
parada de emergencia.

Rt sirve para reiniciar el proceso en caso de que se haya detenido por alguna
alarma o interrupción.
