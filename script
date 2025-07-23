/** script.js COMPLETO **/
const malla = [
  {
    semestre: "1er Semestre",
    ramos: [
      { nombre: "Educación, Cultura y Naturaleza", codigo: "ICED066" },
      { nombre: "Bases Teóricas del Lenguaje y la Comunicación", codigo: "ILLI060" },
      { nombre: "Introducción a los Estudios Literarios", codigo: "ILLI065" },
      { nombre: "Taller de las Artes Escénicas", codigo: "ILLI070" },
      { nombre: "Taller de Nivelación y Acompañamiento", codigo: "ILLI075" },
      { nombre: "Evaluación Inicial Diagnóstica", codigo: "PLAC000" },
      { nombre: "Introducción a las Ciencias Sociales", codigo: "PLAC074" },
      { nombre: "Lectura Comprensiva y Expresión Escrita", codigo: "PLAC093" },
      { nombre: "Comunicación en Lengua Inglesa I", codigo: "PLAC095" },
      { nombre: "Tecnología de la Información y la Comunicación", codigo: "PLAC097" }
    ]
  },
  {
    semestre: "2do Semestre",
    ramos: [
      { nombre: "Educación Física y Salud", codigo: "DYRE070" },
      { nombre: "Aprendizaje y Sistemas de Conocimiento", codigo: "ICED071" },
      { nombre: "Ética, Relacionalidad y Desarrollo Humano", codigo: "ICED082" },
      { nombre: "Fonética Segmental y Suprasegmental", codigo: "ILLI080" },
      { nombre: "Literatura Clásica", codigo: "ILLI085" },
      { nombre: "Práctica de Proyecto Vinculante", codigo: "ILLI090", requisitos: ["ILLI070"] },
      { nombre: "Sociedad y Modernidad", codigo: "PLAC083" },
      { nombre: "Comunicación en Lengua Inglesa II", codigo: "PLAC114", requisitos: ["PLAC095"] }
    ]
  },
  {
    semestre: "3er Semestre",
    ramos: [
      { nombre: "Optativo de Formación General I", codigo: "ELECT127" },
      { nombre: "Taller de Formación General II", codigo: "ELECT066" },
      { nombre: "Aprendizaje, Cognición y Diversidad", codigo: "ICED087", requisitos: ["ICED071"] },
      { nombre: "Currículo, Democracia y Transformación Social", codigo: "ICED093" },
      { nombre: "Taller de Formación Situada: Contextualización y Agenciamiento", codigo: "ICED096" },
      { nombre: "Gramática Oracional", codigo: "ILLI095" },
      { nombre: "Literatura Universal", codigo: "ILLI097" },
      { nombre: "Sociedad y Cultura", codigo: "PLAC121", requisitos: ["PLAC083"] }
    ]
  },
  {
    semestre: "4to Semestre",
    ramos: [
      { nombre: "Gestión y Proyectos Educativos", codigo: "ICED101" },
      { nombre: "Educación Inclusiva", codigo: "ICED107" },
      { nombre: "Gramática Discursiva", codigo: "ILLI110" },
      { nombre: "Semántica General", codigo: "ILLI115" },
      { nombre: "Taller de Formación de Mediadores Lectores", codigo: "ILLI125" },
      { nombre: "Taller de Práctica Inicial", codigo: "ILLI130", requisitos: ["ILLI090", "ICED096"] },
      { nombre: "Didáctica I: Bases Generales", codigo: "ILLI135" },
      { nombre: "Creatividad, Innovación y Proyectos", codigo: "PLAC125", requisitos: ["PLAC093", "PLAC095", "PLAC097", "PLAC114", "PLAC121", "PLAC083"] }
    ]
  },
  {
    semestre: "5to Semestre",
    ramos: [
      { nombre: "Mediaciones TIC y Ambientes de Aprendizaje", codigo: "ICED139" },
      { nombre: "Convivencia Escolar", codigo: "ICED150" },
      { nombre: "Pragmática del Discurso", codigo: "ILLI141" },
      { nombre: "Teoría de la Argumentación", codigo: "ILLI145" },
      { nombre: "Teoría Literaria", codigo: "ILLI151" },
      { nombre: "Práctica de Especialidad: Educación No Formal", codigo: "ILLI160", requisitos: ["ILLI125"] },
      { nombre: "Didáctica II: Literatura, Lengua y Medios", codigo: "ILLI165", requisitos: ["ILLI135"] }
    ]
  },
  {
    semestre: "6to Semestre",
    ramos: [
      { nombre: "Optativo de Especialización I", codigo: "ELECT100" },
      { nombre: "Optativo de Especialización II", codigo: "ELECT101" },
      { nombre: "Evaluación de Aprendizajes", codigo: "ICED156" },
      { nombre: "Género Discursivo y Textos Multimodales", codigo: "ILLI168" },
      { nombre: "Literatura Latinoamericana Colonial y Moderna", codigo: "ILLI173" },
      { nombre: "Práctica de Especialidad: Argumentación", codigo: "ILLI175", requisitos: ["ILLI145"] },
      { nombre: "Didáctica III: Literatura, Lengua y Medios", codigo: "ILLI182", requisitos: ["ILLI165"] }
    ]
  },
  {
    semestre: "7mo Semestre",
    ramos: [
      { nombre: "Optativo de Especialización III", codigo: "ELECT111" },
      { nombre: "Optativo de Especialización IV", codigo: "ELECT118" },
      { nombre: "Taller de Formación Situada: Acompañamiento Reflexivo-Critico", codigo: "ICED192", requisitos: ["ICED096"] },
      { nombre: "Historia de la Lengua", codigo: "ILLI185" },
      { nombre: "Literatura y Perspectivas de Género", codigo: "ILLI188" },
      { nombre: "Literatura Latinoamericana Contemporánea", codigo: "ILLI190" },
      { nombre: "Didáctica IV: Integrada", codigo: "ILLI194", requisitos: ["ILLI182"] }
    ]
  },
  {
    semestre: "8vo Semestre",
    ramos: [
      { nombre: "Optativo de Especialización V", codigo: "ELECT129" },
      { nombre: "Optativo de Especialización VI", codigo: "ELECT130" },
      { nombre: "Metodología de Investigación Educativa", codigo: "ICED195" },
      { nombre: "Variaciones del Español", codigo: "ILLI197" },
      { nombre: "Literatura Chilena", codigo: "ILLI200" },
      { nombre: "Medios de Comunicación", codigo: "ILLI202" },
      { nombre: "Taller de Práctica Intermedia", codigo: "ILLI204", requisitos: ["ICED192"] }
    ]
  },
  {
    semestre: "9no Semestre",
    ramos: [
      { nombre: "Optativo de Profundización I", codigo: "ELECT112", requisitos: ["ICED150", "ILLI165", "ILLI182", "ILLI194", "ICED156", "ILLI168", "ILLI185", "ILLI200", "ILLI173", "ILLI190", "ILLI188", "ICED139", "ILLI202", "ICED195", "ELECT100", "ELECT101", "ELECT111", "ELECT118", "ELECT129", "ELECT130", "ILLI141", "ILLI160", "ILLI145", "ILLI151", "ILLI197", "ICED192", "ILLI204"] },
      { nombre: "Optativo de Profundización II", codigo: "ELECT116", requisitos: ["ICED150", "ILLI165", "ILLI182", "ILLI194", "ICED156", "ILLI168", "ILLI185", "ILLI200", "ILLI173", "ILLI190", "ILLI188", "ICED139", "ILLI202", "ICED195", "ELECT100", "ELECT101", "ELECT111", "ELECT118", "ELECT129", "ELECT130", "ILLI141", "ILLI160", "ILLI145", "ILLI151", "ILLI197", "ICED192", "ILLI204"] },
      { nombre: "Seminario de Investigación", codigo: "ILLI206", requisitos: ["ICED150", "ILLI165", "ILLI182", "ILLI194", "ICED156", "ILLI168", "ILLI185", "ILLI200", "ILLI173", "ILLI190", "ILLI188", "ICED139", "ILLI202", "ICED195", "ELECT100", "ELECT101", "ELECT111", "ELECT118", "ELECT129", "ELECT130", "ILLI141", "ILLI160", "ILLI145", "ILLI151", "ILLI197", "ICED192", "ILLI204"] },
      { nombre: "Taller de Consolidación Profesional", codigo: "ILLI208" },
      { nombre: "Taller de Formación Situada: Desarrollo Profesional y Aprendizaje Servicio", codigo: "ILLI210", requisitos: ["ICED150", "ILLI165", "ILLI182", "ILLI194", "ICED156", "ILLI168", "ILLI185", "ILLI200", "ILLI173", "ILLI190", "ILLI188", "ICED139", "ILLI202", "ICED195", "ELECT100", "ELECT101", "ELECT111", "ELECT118", "ELECT129", "ELECT130", "ILLI141", "ILLI160", "ILLI145", "ILLI151", "ILLI197", "ICED192", "ILLI204"] }
    ]
  },
  {
    semestre: "10mo Semestre",
    ramos: [
      { nombre: "Práctica Profesional", codigo: "ILLI295", requisitos: ["ILLI208", "ILLI210"] },
      { nombre: "Seminario de Titulación", codigo: "ILLI299", requisitos: ["ILLI206"] }
    ]
  }
];

const estadoRamos = {};

function crearCheckbox(ramo) {
  const div = document.createElement('div');
  div.className = 'ramo';
  if (ramo.requisitos) {
    div.classList.add('disabled');
  }

  const label = document.createElement('label');
  label.innerText = `${ramo.nombre} (${ramo.codigo})`;

  const checkbox = document.createElement('input');
  checkbox.type = 'checkbox';
  checkbox.disabled = !!ramo.requisitos;
  checkbox.id = ramo.codigo;

  checkbox.addEventListener('change', () => {
    estadoRamos[ramo.codigo] = checkbox.checked;
    actualizarEstado();
  });

  div.appendChild(label);
  div.appendChild(checkbox);

  return div;
}

function actualizarEstado() {
  document.querySelectorAll('.ramo').forEach(div => {
    const id = div.querySelector('input').id;
    const ramo = encontrarRamo(id);
    if (ramo.requisitos) {
      const habilitado = ramo.requisitos.every(req => estadoRamos[req]);
      const checkbox = div.querySelector('input');
      checkbox.disabled = !habilitado;
      div.classList.toggle('disabled', !habilitado);
    }
  });
}

function encontrarRamo(codigo) {
  for (const sem of malla) {
    for (const ramo of sem.ramos) {
      if (ramo.codigo === codigo) return ramo;
    }
  }
  return null;
}

function renderMalla() {
  const container = document.getElementById('malla-container');
  malla.forEach(semestre => {
    const semDiv = document.createElement('div');
    semDiv.className = 'semestre';

    const h2 = document.createElement('h2');
    h2.textContent = semestre.semestre;
    semDiv.appendChild(h2);

    semestre.ramos.forEach(ramo => {
      const checkbox = crearCheckbox(ramo);
      semDiv.appendChild(checkbox);
    });

    container.appendChild(semDiv);
  });
}

document.addEventListener('DOMContentLoaded', () => {
  renderMalla();
});
