Ejercicio Next.js
Este es mi ejercicio realizado en Next.js.
ejercicio-next.js

codigo sugerio para el ejercico rempazar el archivo page.tsx por este

"use client";

import { useState } from "react";

export default function Inicio() {
  // Estado para guardar la tarea que se está escribiendo
  const [tarea, setTarea] = useState(____);

  // Lista inicial de tareas
  const [tareas, setTareas] = useState([
    "Estudiar Next.js",
    "Realizar el ejercicio",
    "Practicar programación",
  ]);

  function agregarTarea() {
    // Verificar que la tarea no esté vacía
    if (________) {
      // Agregar la nueva tarea a la lista
      setTareas(__________);

      // Limpiar el input después de agregar
      setTarea(____);
    }
  }

  return (
    <main>
      <h1>Mis tareas</h1>

      <div className="formulario">
        <input
          type="text"
          placeholder="Escribe una tarea"
          value={____}
          onChange={(e) => ________}
        />

        <button onClick={______}>
          Agregar
        </button>
      </div>

      <ul>
        {tareas.____((tarea, index) => (
          <li key={___}>{___}</li>
        ))}
      </ul>
    </main>
  );
}
