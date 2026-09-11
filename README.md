# practica6_253239

1. ¿Qué pasaría si el módulo no quedara registrado en la raíz?
Si no registrara el modulo Nest ni se enteraria de que mi controlador existe y aunque el archivo este ahi guardado la ruta simplemente no funcionaria y me daría un error
de "no encontrado" como si nunca la hubiera escrito

2. ¿Por qué los métodos del repositorio devuelven promesas si los datos van a estar en memoria?
Aunque ahorita los datos solo viven en un arreglo y no tardan nada en consultarse lo deje preparado por si algun dia fuera a conectarse a una base de datos real
que esa si tardaria en responder entoces si se cambia a una base de datos de verdad no tengo que rehacer todo porque ya estaba pensado para eso desde el principio

3. ¿Qué error apareció al cambiar a la interfaz, y por qué la clase sí se había resuelto sola?
Me salio un error diciendo que Nest no podia encontrar de donde sacar esa pieza

4. ¿Por qué el servicio necesita un token para el repositorio, pero el controlador no lo necesita para el servicio?
El servicio si sigue existiendo cuando el programa corre entonces pues el Nest lo encuentra solo sin ayuda extra

5. ¿Cuál es la diferencia entre un 400 y un 409?
El 400 es cuando se mandan mal los datos desde un inicio o se pone el tipo de dato equivocado y ps "truena"
El 409 es cuando los datos estan bien pero no se pueden aplicar porque chocan con algo que ya existe como intentar apuntarme dos veces a la misma clase
o cuando ya no hay lugar como se ven en las capturas de la practica

6. ¿Por qué cambió el código de estado de esa última petición?
Porque al cancelar una inscripcion esa persona deja de contar para el cupo del horario y mi codigo solo cuenta las inscripciones que siguen activas así que en cuanto
cancele una se libero un lugar y la misma peticion que antes fallaba por falta de cupo y ps esta vez si pudo pasar
