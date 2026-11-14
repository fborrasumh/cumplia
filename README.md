# CumplIA

La consulta en regla: publicidad, unidad U.48, datos de pacientes e imágenes. Aplicación web de un solo fichero.

**Usar la app:** https://fborrasumh.github.io/cumplia/

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24214569.svg)](https://doi.org/10.5281/zenodo.24214569)

**Idiomas:** español (por defecto), inglés y portugués. Se cambian con el selector de la barra superior o con `?lang=en` / `?lang=pt` en la URL.

## Qué hace

Es la séptima y última app del [Kit EstéticIA](https://fborrasumh.github.io/kitesteticia/).

- **Revisor de publicaciones.** Pegas el texto de una publicación y marcas si incluye fotos de antes y después, un paciente identificable o una colaboración pagada. La app marca en el texto:
  - medicamentos de prescripción y marcas de toxina botulínica;
  - marcas de productos sanitarios;
  - promesas de resultado o de seguridad, y propiedades adelgazantes;
  - sorteos, precios y ofertas, y presión comercial;
  - testimonios y superlativos;
  - la falsa «especialidad en medicina estética»;
  - la falta del número de colegiado o del número de registro sanitario;
  - fotos de pacientes sin consentimiento y publicidad encubierta.

  Cada alerta lleva su porqué, la norma y una alternativa. Rojo significa que la práctica está prohibida por una norma; ámbar, que es contraria al Código de Deontología Médica o que falta un dato. Hay un registro de las publicaciones revisadas.
- **Lista de la unidad U.48**: autorización y personal, historia clínica y consentimiento, medicamentos y productos sanitarios, urgencias, equipos, limpieza y residuos, y publicidad. Cada punto se marca como «Cumplo», «Pendiente» o «No aplica», con su norma.
- **Lista de protección de datos** para una consulta que trata datos de salud.
- **Consentimiento para el uso de imágenes**: cada uso se autoriza por separado, se elige qué se puede mostrar y durante cuánto tiempo, y es revocable. Avisa en el caso de menores. El documento sale en Word, en español, inglés o portugués, y puede tomar el identificador de una ficha de AnamnesIA.
- **Plan de cumplimiento** en Word: lo pendiente con su norma y el registro de revisiones.

No usa IA y no hace ninguna llamada de red. Las reglas son patrones escritos, así que lo que no está en ellas no se detecta.

## Normativa

- RD 1907/1996 (publicidad con pretendida finalidad sanitaria), RDL 1/2015 (art. 80) y RD 1591/2009 (arts. 38-40).
- RD 1277/2003 (anexo II, U.48); en la Comunitat Valenciana, Decreto 157/2014 y Orden 7/2017.
- Código de Deontología Médica (CGCOM, 2022), Ley 41/2002 y Ley 44/2003.
- RGPD, LOPDGDD, LO 1/1982, Ley 3/1991 y LSSI.
- Como modelo de lista: la guía de inspección de centros de medicina estética de la Junta de Andalucía (2024).

## Límites

Es una herramienta de apoyo para médicos y no es asesoramiento jurídico. La normativa autonómica puede exigir más. En la Comunitat Valenciana, la Conselleria de Sanidad ha abierto consulta pública para una orden con requisitos específicos de medicina estética.

## Pruebas

- `node tests/test_nucleo.js` comprueba las reglas en los tres idiomas, los límites de palabra, el contexto de la publicación, las listas, el consentimiento y el plan.
- `python3 tests/smoke.py` hace el recorrido completo: foco al escribir, registro, Word, ficha de AnamnesIA, persistencia, tres idiomas, accesibilidad WCAG 2.2 AA, CSP y móvil.

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche) y Elena Caride Miana (Dra. Caride Medicina Estética & Antiaging).

Séptima y última app del Kit EstéticIA, diseñado para el alumnado del Máster de Formación Permanente en Medicina Estética Integral y Antienvejecimiento (UMH).

ORCID: Fernando Borrás Rocher [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573) · Elena Caride Miana [0000-0002-7620-4857](https://orcid.org/0000-0002-7620-4857)

## Cómo citar

Borrás Rocher, F. y Caride Miana, E. (2026). *CumplIA* (v1.0.0) [Software]. DOI: [10.5281/zenodo.24214569](https://doi.org/10.5281/zenodo.24214569)

## Licencia

MIT. Véase [LICENSE](LICENSE).
