		TAREA #01: MIXED Y SOFT

Se analizara como sirven los comandos ya mencionados ligado 
al tema de "Deshaciendo Cambios".

	git reset [<mode>][<commit>]

La anterior linea de codigo se restablece la branch head 
(cabeza rama) actual a <commit> y posiblemente actualiza 
el indice (que permanezca en el árbol de <commit>) y el
árbol de trabajo en funcion de <mode>, por defecto es 
"--mixed" .El <mode> debe ser uno de los siguientes:

--SOFT:
  No toca el archivo de índice o el árbol de trabajo en 
  absoluto (pero restablece la cabeza/head a <commit>,
  al igual que todos los modos de hacer). Esto deja a 
  todos sus archivos modificados "Los cambios que se 
  cometan", como git status lo pondría.

--MIXED:
  Restablece el índice, pero no el árbol de trabajo (es 
  decir, los archivos modificados se conservan pero no 
  marcados para el commit) e informa de lo que no se ha 
  actualizado. Esta es la acción por defecto.
  Si -N es especificada, los caminos removidos son 
  marcados como por intención de sumar (intent-to-add).
  Se puede ver mas a fondo en git -add.
