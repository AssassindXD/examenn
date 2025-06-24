
# Prueba para Pasantía Técnica UNCPGGL

## 📘 Prueba de SQL

### 🧾 Instrucciones
Resuelva las siguientes consultas utilizando **SQL**. Puede usar SQLite o cualquier otro gestor compatible. Se evaluará:
- Correcta estructura de las consultas
- Uso adecuado de `JOIN`, `GROUP BY`, `HAVING`, etc.
- Claridad y comentarios si son necesarios

---

### 🟢 Nivel Básico

1. **Listado de estudiantes**  
   Muestra todos los estudiantes registrados con su nombre completo, identificación, sexo y fecha de nacimiento.
 <!--select * from students      bueno--> 
2. **Buscar estudiantes por sexo**  
   Muestra todos los estudiantes de sexo femenino (`F`).
<!--  select * from estudents where sex= 'F';    bueno --> 
3. **Contar estudiantes por sexo**  
   ¿Cuántos hombres y mujeres hay en total?
<!--   select sex, count(*) from students group by sex      bueno--> 
4. **Carreras disponibles**  
   Lista todas las carreras disponibles en la base de datos.
<!--  select * from careers  bueno --> 
5. **Consulta de régimen**  
   ¿Cuáles son los tipos de régimen académico registrados?
<!--  select(*)from academic_regime; bueno  --> 
---

### 🟡 Nivel Intermedio

6. **Matriculados por año**  
   ¿Cuántos estudiantes se matricularon en el año 2024?
   <!--  select year, count(*) from enrollments group by year= '2024'      bueno  --> 

7. **Cantidad de repitentes**  
   ¿Cuántos estudiantes están repitiendo (`repeater = true`)?
   <!-- select count * from students where repeater = 1;  malo --> 

8. **Estudiantes con más de una matrícula**  
   Muestra los estudiantes que tienen más de una matrícula, incluyendo su nombre y el número de matrículas.

9. **Materias inscritas por estudiante**  
   Dado el nombre completo de un estudiante, muestra todas las materias que ha inscrito (con período y año).

10. **Notas registradas**  
    Muestra todas las inscripciones que tienen nota registrada (nombre del estudiante, materia, nota).

---

### 🔴 Nivel Avanzado

11. **Promedio de notas por estudiante**  
    Calcula el promedio de nota de cada estudiante que tenga al menos una nota registrada.

12. **Estudiantes sin notas**  
    Muestra los estudiantes que no tienen ninguna nota en ninguna de sus inscripciones.

13. **Cantidad de materias por matrícula**  
    ¿Cuántas materias inscritas hay por cada matrícula? Muestra el ID de matrícula, nombre del estudiante y el total.

14. **Top 10 estudiantes con mejor promedio**  
    Lista los 10 estudiantes con mayor promedio de notas.

15. **Estudiantes con materias inscritas en más de un régimen**  
    Muestra los estudiantes que tienen matrículas en más de un régimen académico distinto (por ejemplo: en semestral y cuatrimestral).

---

### 🧠 Extra (Bonus)

16. **Simulación de boletín**  
    Para un estudiante específico, muestra un resumen con:
    - Año y período
    - Carrera y curso
    - Materia inscrita
    - Nota (si tiene)

17. **Detección de materias repetidas**  
    ¿Hay materias que un estudiante ha inscrito más de una vez en distintos años o períodos?

18. **Porcentaje de estudiantes por régimen**  
    ¿Qué cantidad de estudiantes está en cada tipo de régimen académico?

19. **Distribución de estudiantes por turno**  
    ¿Cuántos estudiantes hay por turno (mañana, tarde, noche)?

20. **Promedio de notas por carrera**  
    Muestra el promedio de notas agrupado por carrera.

---

## 📘 Prueba de Maquetacion

Cree una página HTML utilizando **Bootstrap 5** que contenga un formulario de matrícula de estudiante. El formulario debe ser responsivo y estar correctamente maquetado utilizando el sistema de grid y componentes de formularios de Bootstrap. Debe tomar en cuenta los campos de la tabla `enrollments` y  `students`

## 📘 Consumo de API REST (JavaScript Fetch)

Usando HTML + JavaScript (vanilla o framework opcional), consuma la siguiente API:

https://jsonplaceholder.typicode.com/users/

### 🧾 Requisitos del ejercicio:   

1. Realiza una solicitud GET a la API.
2. Muestra los usuarios en pantalla en una tabla o tarjeta.
3. Por cada usuario, debes mostrar:
    - Nombre
    - Correo electrónico
    - Teléfono
    - Ciudad (desde address.city)
    - Empresa (desde company.name)

Agrega un botón que permita recargar los datos (vuelve a hacer fetch).

---

## 🧠 Extras

1. Utilizar buenas practicas al realizar commits
2. Subir el proyecto a GitHub
3. Hacer uso de algún Framework o motor de plantillas   
         
---

✍️ *Buena suerte y recuerda justificar tu lógica cuando sea necesario.*