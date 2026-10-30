# Extremadura: law history in git

The law of the autonomous community of Extremadura (Comunidad Autónoma de Extremadura, Spain) as a git history: one file per article, one commit per norm that changed it, dated the day the change took effect, with the amending norm as the commit's author. `git blame` names the norm behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `es-ex/`. Spain's national law is in [lexifina/spain-law](https://github.com/lexifina/spain-law).

The text is in Spanish, exactly as the BOE's consolidated text prints it. Texts in co-official languages are not included.

Basado en datos de la Agencia Estatal Boletín Oficial del Estado (<https://www.boe.es>). Every text here is a consolidated text for information only (texto consolidado de carácter meramente informativo), not an official publication.

## What this repository holds

181 norms with 567 versions so far: the Estatuto de Autonomía first, then the laws, decree-laws and legislative decrees in force that the BOE consolidates, oldest first, added in parts of about 50. 15 of them are repealed norms the BOE consolidates: their whole history is kept, and their last commit removes the text on the day the repeal took effect, credited to the repealing norm. Regulations are not included (the BOE consolidates no autonomic decrees or orders).

| Folder | Norm | Versions | History | BOE last updated |
| --- | --- | ---: | --- | --- |
| `estatuto-de-autonomia/` | Ley Orgánica 1/2011, de 28 de enero, de reforma del Estatuto de Autonomía de la Comunidad Autónoma de Extremadura. | 1 | as first published: 29 January 2011 | 2026-10-30 |
| `ley-1985-004/` | Ley 4/1985, de 3 de junio, del Escudo, Himno y día de Extremadura. | 1 | as first published: 15 June 1985 | 2026-01-15 |
| `ley-1985-007/` | Ley 7/1985, de 26 de noviembre, de Iniciativa Legislativa Popular de la Comunidad Autónoma de Extremadura. | 1 | as first published: 23 December 1985 | 2025-12-17 |
| `ley-1986-001/` | Ley 1/1986, de 2 de mayo, sobre la Dehesa en Extremadura. | 3 | as first published, then each change: 4 June 1986 to 26 June 2015 | 2025-12-17 |
| `ley-1987-002/` | Ley 2/1987, de 16 de marzo, de Elecciones a la Asamblea de Extremadura. | 2 | as first published, then each change: 16 March 1987 to 26 March 1991 | 2025-12-17 |
| `ley-1989-003/` | Ley 3/1989, de 27 de diciembre, de Capitalidad de los Partidos Judiciales de Extremadura. | 1 | as first published: 3 January 1990 | 2025-12-17 |
| `ley-1990-002/` | Ley 2/1990, de 26 de abril, de Salud Escolar. | 1 | as first published: 20 June 1990 | 2025-12-17 |
| `ley-1991-001/` | Ley 1/1991, de 7 de marzo, reguladora de régimen jurídico de los baldíos de Alburquerque. | 1 | as first published: 27 March 1991 | 2025-12-17 |
| `ley-1991-003/` | Ley 3/1991, de 25 de abril, de creación del Consejo Económico y Social de Extremadura. | 5 | as first published, then each change: 10 May 1991 to 30 November 2022 | 2025-12-17 |
| `ley-1994-002/` | Ley 2/1994, de 28 de abril, de asistencia social geriátrica. | 1 | as first published: 20 May 1994 | 2025-12-17 |
| `ley-1994-003/` | Ley 3/1994, de 26 de mayo, de Artesanía de la Comunidad Autónoma de Extremadura. | 1 | as first published: 4 July 1994 | 2025-12-17 |
| `ley-1994-004/` | Ley 4/1994, de 10 de noviembre, de protección y atención a menores. | 1 | as first published: 25 November 1994 | 2025-12-17 |
| `ley-1994-006/` | Ley 6/1994, de 24 de noviembre, de Balnearios y de Aguas Minero-Medicinales y/o Termales. | 1 | as first published: 23 December 1994 | 2025-12-18 |
| `ley-1994-008/` | Ley 8/1994, de 23 de diciembre, de Cajas de Ahorros. | 5 | as first published, then each change: 22 January 1995 to 12 February 2015 | 2025-12-18 |
| `ley-1995-002/` | Ley 2/1995, de 6 de abril, del Deporte de Extremadura. | 3 | as first published, then each change: 30 April 1995 to 10 April 2019 | 2025-12-18 |
| `ley-1995-007/` | Ley 7/1995, de 27 de abril, de Carreteras de Extremadura. | 3 | as first published, then each change: 5 June 1995 to 16 May 2018 | 2025-12-18 |
| `ley-1997-003/` | Ley 3/1997, de 20 de marzo, de Extinción de Cámaras Agrarias Locales. | 2 | as first published, then each change: 30 April 1997 to 1 January 2003 | 2025-12-18 |
| `ley-1998-005/` | Ley 5/1998, de 18 de junio, de creación del Colegio Oficial de Podólogos de la Comunidad Autónoma de Extremadura. | 1 | as first published: 19 July 1998 | 2025-12-18 |
| `ley-1998-006/` | Ley 6/1998, de 18 de junio, del Juego de Extremadura. | 13 | as first published, then each change: 7 August 1998 to 8 February 2019 | 2025-12-18 |
| `ley-1998-008/` | Ley 8/1998, de 26 de junio, de Conservación de la Naturaleza y de Espacios Naturales de Extremadura. | 7 | as first published, then each change: 28 August 1998 to 23 September 2025 | 2026-10-14 |
| `ley-1999-001/` | Ley 1/1999, de 29 de marzo, de Prevención, Asistencia y Reinserción de las Drogodependencias de la Comunidad Autónoma de Extremadura. | 3 | as first published, then each change: 21 April 1999 to 30 November 2022 | 2025-12-18 |
| `ley-1999-002/` | Ley 2/1999, de 29 de marzo, de Patrimonio Histórico y Cultural de Extremadura. | 10 | as first published, then each change: 23 May 1999 to 30 November 2022 | 2026-10-27 |
| `ley-2000-001/` | Ley 1/2000, de 16 de marzo, de creación del Colegio Profesional de Protésicos Dentales de Extremadura. | 1 | as first published: 12 April 2000 | 2025-12-18 |
| `ley-2001-005/` | Ley 5/2001, de 10 de mayo, de Crédito Cooperativo. | 7 | as first published, then each change: 8 June 2001 to 30 November 2022 | 2025-12-18 |
| `ley-2001-007/` | Ley 7/2001, de 14 de junio, de creación del Servicio Extremeño Público de Empleo. | 3 | as first published, then each change: 4 July 2001 to 9 May 2019 | 2025-12-18 |
| `ley-2001-008/` | Ley 8/2001, de 14 de junio, por la que se regulan los Consejos Escolares de Extremadura. | 3 | as first published, then each change: 4 July 2001 to 5 November 2020 | 2025-12-18 |
| `ley-2001-009/` | Ley 9/2001, de 28 de junio, de creación del Colegio Profesional de Fisioterapeutas de Extremadura. | 1 | as first published: 4 July 2001 | 2025-12-18 |
| `ley-2001-010/` | Ley 10/2001, de 28 de junio, de Salud de Extremadura. | 5 | as first published, then each change: 4 July 2001 to 1 January 2019 | 2025-12-18 |
| `ley-2001-011/` | Ley 11/2001, de 10 de octubre, de creación del Instituto de la Mujer de Extremadura. | 1 | as first published: 9 November 2001 | 2025-12-18 |
| `ley-2002-001/` | Ley 1/2002, de 28 de febrero, del Gobierno y de la Administración de la Comunidad Autónoma de Extremadura. | 9 | as first published, then each change: 27 March 2002 to 30 November 2022 | 2026-10-30 |
| `ley-2002-002/` | Ley 2/2002, de 25 de abril, de Protección de la Calidad del Suministro Eléctrico en Extremadura. | 5 | as first published, then each change: 3 June 2002 to 23 November 2018 | 2025-12-18 |
| `ley-2002-003/` | Ley 3/2002, de 9 de mayo, de Comercio, de la Comunidad Autónoma de Extremadura. | 9 | as first published, then each change: 17 June 2002 to 27 October 2018 | 2025-12-18 |
| `ley-2002-005/` | Ley 5/2002, de 23 de mayo, de Protección de los Animales en la Comunidad Autónoma de Extremadura. | 4 | as first published, then each change: 18 September 2002 to 30 April 2019 | 2026-10-13 |
| `ley-2002-009/` | Ley 9/2002, de 14 de noviembre, de Impulso a la Localización Industrial de Extremadura. | 2 | as first published, then each change: 15 December 2002 to 9 May 2019 | 2025-12-18 |
| `ley-2002-010/` | Ley 10/2002, de 12 de diciembre, de Financiación de Inversiones Extraordinarias. | 1 | as first published: 14 December 2002 | 2025-12-18 |
| `ley-2002-011/` | Ley 11/2002, de 12 de diciembre, de Colegios y de Consejos de Colegios Profesionales de Extremadura. | 3 | as first published, then each change: 29 December 2002 to 24 November 2020 | 2025-12-18 |
| `ley-2003-003/` | Ley 3/2003, de 13 de marzo, sobre participación institucional de los agentes sociales más representativos. | 2 | as first published, then each change: 11 April 2003 to 1 January 2010 | 2025-12-18 |
| `ley-2003-004/` | Ley 4/2003, de 20 de marzo, de Estadística de la Comunidad Autónoma de Extremadura. | 3 | as first published, then each change: 9 April 2003 to 30 November 2022 | 2025-12-18 |
| `ley-2003-005/` | Ley 5/2003, de 20 de marzo, de parejas de hecho de la Comunidad Autónoma de Extremadura. | 1 | as first published: 9 April 2003 | 2025-12-18 |
| `ley-2004-005/` | Ley 5/2004, de 24 de junio, de prevención y lucha contra los incendios forestales en Extremadura. | 5 | as first published, then each change: 30 June 2004 to 31 March 2023 | 2025-12-18 |
| `ley-2004-007/` | Ley 7/2004, de 19 de noviembre, por la que se declara a Cornalvo Parque Natural. | 1 | as first published: 1 December 2004 | 2025-12-18 |
| `ley-2004-008/` | Ley 8/2004, de 23 de diciembre, para la aplicación al municipio de Mérida, capital de Extremadura, del régimen de organización de los municipios de gran población contemplado en el título X de la Ley 7/1985, de 2 de abril, Reguladora de las Bases de Régimen Local, modificada por la Ley 57/2003, de 16 de diciembre, de Medidas para la Modernización del Gobierno Local. | 1 | as first published: 31 December 2004 | 2025-12-18 |
| `ley-2005-001/` | Ley 1/2005, de 24 de junio, de tiempos de respuesta en la atención sanitaria especializada del sistema sanitario público de Extremadura. | 1 | as first published: 7 October 2005 | 2026-06-26 |
| `ley-2005-002/` | Ley 2/2005, de 24 de junio, de creación del Jurado de Defensa de la Competencia de Extremadura. | 3 | as first published, then each change: 27 July 2005 to 30 November 2022 | 2025-12-18 |
| `ley-2005-003/` | Ley 3/2005, de 8 de julio, de información sanitaria y autonomía del paciente. | 1 | as first published: 5 August 2005 | 2025-12-18 |
| `ley-2005-004/` | Ley 4/2005, de 8 de julio, de reordenación del sector público empresarial de la Comunidad Autónoma de Extremadura. | 4 | as first published, then each change: 17 July 2005 to 21 February 2014 | 2025-12-18 |
| `ley-2005-006/` | Ley 6/2005, de 27 de diciembre, de medidas para la asistencia y atención de las víctimas del terrorismo y de creación del Centro Extremeño de Estudios para la Paz. | 2 | as first published, then each change: 1 January 2006 to 10 March 2020 | 2025-12-18 |
| `ley-2006-001/` | Ley 1/2006, de 7 de julio, por la que se declara el Parque Natural del «Tajo internacional». | 1 | as first published: 9 July 2006 | 2025-12-18 |
| `ley-2006-004/` | Ley 4/2006, de 10 de octubre, por la que se crea el Colegio Profesional de Terapeutas Ocupacionales de Extremadura. | 1 | as first published: 22 October 2006 | 2025-12-18 |
| `ley-2006-005/` | Ley 5/2006, de 10 de octubre, por la que se crea el Colegio Profesional de Ingenieros en Informática de Extremadura. | 1 | as first published: 22 October 2006 | 2025-12-18 |
| `ley-2006-006/` | Ley 6/2006, de 9 de noviembre, de Farmacia de Extremadura. | 3 | as first published, then each change: 17 November 2006 to 30 November 2022 | 2025-12-18 |
| `decreto-legislativo-2006-002/` | Decreto Legislativo 2/2006, de 12 de diciembre, por el que se aprueba el Texto Refundido de las disposiciones legales de la comunidad autónoma de Extremadura en materia de Tributos Propios. | 10 | oldest version available, then each change: 24 December 2006 to 27 April 2025 | 2025-04-14 |
| `ley-2006-008/` | Ley 8/2006, de 23 diciembre, de Sociedades Cooperativas Especiales de Extremadura. | 2 | as first published, then each change: 19 January 2007 to 2 January 2019 | 2025-12-19 |
| `ley-2007-001/` | Ley 1/2007, de 20 de marzo, de creación del Instituto de la Juventud de Extremadura. | 2 | as first published, then each change: 16 April 2007 to 9 May 2019 | 2025-12-19 |
| `ley-2007-002/` | Ley 2/2007, de 12 de abril, de Archivos y Patrimonio Documental de Extremadura. | 2 | as first published, then each change: 16 May 2007 to 9 May 2019 | 2025-12-19 |
| `ley-2007-004/` | Ley 4/2007, de 19 de abril, por la que se crea el Colegio Profesional de Técnicos Superiores en Imagen para el Diagnóstico de Extremadura. | 1 | as first published: 29 April 2007 | 2025-12-19 |
| `ley-2007-005/` | Ley 5/2007, de 19 de abril, General de Hacienda Pública de Extremadura. | 17 | as first published, then each change: 28 August 2007 to 5 August 2026 | 2026-08-17 |
| `ley-2008-001/` | Ley 1/2008, de 22 de mayo, de creación de Entidades Públicas de la Junta de Extremadura. | 10 | as first published, then each change: 27 May 2008 to 1 April 2023 | 2025-12-19 |
| `ley-2008-002/` | Ley 2/2008, de 16 de junio, de Patrimonio de la Comunidad Autónoma de Extremadura. | 6 | as first published, then each change: 17 August 2008 to 30 November 2022 | 2025-12-19 |
| `ley-2008-003/` | Ley 3/2008, de 16 de junio, reguladora de la Empresa Pública «Corporación Extremeña de Medios Audiovisuales». | 2 | as first published, then each change: 17 June 2008 to 1 January 2011 | 2025-12-19 |
| `ley-2008-004/` | Ley 4/2008, de 25 de noviembre, de endeudamiento extraordinario de la Comunidad Autónoma de Extremadura. | 1 | as first published: 26 November 2008 | 2025-12-19 |
| `ley-2009-001/` | Ley 1/2009, de 18 de febrero, de creación del Colegio Profesional de Educadoras y Educadores Sociales de Extremadura. | 1 | as first published: 21 February 2009 | 2025-12-19 |
| `ley-2009-002/` | Ley 2/2009, de 2 de marzo, para la puesta en marcha de un Plan Extraordinario de Apoyo al Empleo Local. | 1 | as first published: 7 March 2009 | 2025-12-19 |
| `ley-2009-003/` | Ley 3/2009, de 22 de junio, de creación del Instituto de Estadística de Extremadura. | 2 | as first published, then each change: 24 June 2009 to 9 May 2019 | 2025-12-19 |
| `ley-2009-005/` | Ley 5/2009, de 25 de noviembre, de medidas urgentes en materia de transporte público regular, permanente y de uso general de viajeros por carretera. | 2 | as first published, then each change: 2 December 2009 to 9 June 2021 | 2025-12-19 |
| `ley-2009-006/` | Ley 6/2009, de 17 de diciembre, del Estatuto de los extremeños en el exterior. | 1 | as first published: 22 December 2009 | 2025-12-19 |
| `ley-2010-001/` | Ley 1/2010, de 7 de enero, del Consejo Social de la Universidad de Extremadura. | 1 | as first published: 1 February 2010 | 2025-12-19 |
| `ley-2010-002/` | Ley 2/2010, de 26 de febrero, de creación del Colegio Profesional de Logopedas de Extremadura. | 4 | as first published, then each change: 3 March 2010 to 1 August 2013 | 2025-12-19 |
| `ley-2010-003/` | Ley 3/2010, de 26 de febrero, de creación del Colegio Profesional de Higienistas Dentales de Extremadura. | 4 | as first published, then each change: 3 March 2010 to 1 August 2013 | 2025-12-19 |
| `ley-2010-004/` | Ley 4/2010, de 28 de abril, de Denominaciones de Origen e Indicaciones Geográficas de Calidad Agroalimentaria de Extremadura. | 3 | as first published, then each change: 20 May 2010 to 20 June 2020 | 2025-12-19 |
| `ley-2010-008/` | Ley 8/2010, de 19 de julio, de Actividades Feriales de la Comunidad Autónoma de Extremadura. | 2 | as first published, then each change: 23 July 2010 to 24 October 2012 | 2025-12-19 |
| `ley-2010-010/` | Ley 10/2010, de 16 de noviembre, de la ciencia, la tecnología y la innovación de Extremadura. | 3 | as first published, then each change: 20 November 2010 to 30 November 2022 | 2025-12-19 |
| `ley-2010-011/` | Ley 11/2010, de 16 de noviembre, de pesca y acuicultura de Extremadura. | 3 | as first published, then each change: 19 February 2011 to 30 November 2022 | 2025-12-19 |
| `ley-2010-012/` | Ley 12/2010, de 16 de noviembre, de impulso al nacimiento y consolidación de empresas en la Comunidad Autónoma de Extremadura. | 3 | as first published, then each change: 9 December 2010 to 29 June 2015 | 2025-12-19 |
| `ley-2010-013/` | Ley 13/2010, de 24 de noviembre, del Consejo de la Juventud de Extremadura. | 3 | as first published, then each change: 27 November 2010 to 21 May 2014 | 2025-12-19 |
| `ley-2010-014/` | Ley 14/2010, de 9 de diciembre, de caza de Extremadura. | 4 | as first published, then each change: 15 June 2011 to 30 November 2022 | 2025-12-19 |
| `ley-2010-015/` | Ley 15/2010, de 9 de diciembre, de responsabilidad social empresarial en Extremadura. | 1 | as first published: 4 January 2011 | 2025-12-19 |
| `ley-2010-016/` | Ley 16/2010, de 21 de diciembre, de actuación integral en zonas de atención especial de la Comunidad Autónoma de Extremadura. | 1 | as first published: 12 January 2011 | 2025-12-19 |
| `ley-2010-017/` | Ley 17/2010, de 22 de diciembre, de mancomunidades y entidades locales menores de Extremadura. | 5 | as first published, then each change: 24 December 2010 to 30 November 2022 | 2025-12-19 |
| `ley-2010-020/` | Ley 20/2010, de 28 de diciembre, de concentración empresarial pública en la Comunidad Autónoma de Extremadura. | 3 | as first published, then each change: 31 December 2010 to 15 December 2016 | 2025-12-19 |
| `ley-2011-002/` | Ley 2/2011, de 31 de enero, de desarrollo y modernización del turismo de Extremadura. | 5 | as first published, then each change: 2 August 2011 to 30 November 2022 | 2025-12-19 |
| `ley-2011-004/` | Ley 4/2011, de 7 de marzo, de educación de Extremadura. | 2 | as first published, then each change: 9 September 2011 to 10 April 2015 | 2026-01-12 |
| `ley-2011-006/` | Ley 6/2011, de 23 de marzo, de subvenciones de la Comunidad Autónoma de Extremadura. | 11 | as first published, then each change: 25 June 2011 to 5 August 2026 | 2026-10-21 |
| `ley-2011-007/` | Ley 7/2011, de 23 de marzo, de salud pública de Extremadura. | 2 | as first published, then each change: 14 April 2011 to 28 July 2020 | 2026-10-14 |
| `ley-2011-008/` | Ley 8/2011, de 23 de marzo, de Igualdad entre mujeres y hombres y contra la violencia de género en Extremadura. | 1 | as first published: 26 March 2011 | 2025-12-19 |
| `ley-2012-002/` | Ley 2/2012, de 28 de junio, de medidas urgentes en materia tributaria, financiera y de juego de la Comunidad Autónoma de Extremadura. | 10 | as first published, then each change: 29 June 2012 to 5 August 2026 | 2026-08-17 |
| `ley-2013-004/` | Ley 4/2013, de 21 de mayo, de Gobierno Abierto de Extremadura. | 6 | as first published, then each change: 24 November 2013 to 30 November 2022 | 2025-12-19 |
| `ley-2013-008/` | Ley 8/2013, de 27 de diciembre, de comunicación y publicidad institucional de Extremadura. | 2 | as first published, then each change: 19 January 2014 to 21 February 2014 | 2025-12-19 |
| `ley-2014-001/` | Ley 1/2014, de 18 de febrero, de regulación del estatuto de los cargos públicos del Gobierno y la Administración de la Comunidad Autónoma de Extremadura. | 6 | as first published, then each change: 21 May 2014 to 28 July 2023 | 2025-12-19 |
| `ley-2014-008/` | Ley 8/2014, de 1 de octubre, por la que se establece un marco de financiación estable para la Universidad de Extremadura. | 1 | as first published: 23 October 2014 | 2025-12-19 |
| `ley-2014-011/` | Ley 11/2014, de 9 de diciembre, de accesibilidad universal de Extremadura. | 2 | as first published, then each change: 12 December 2014 to 30 November 2022 | 2025-12-19 |
| `ley-2015-001/` | Ley 1/2015, de 10 de febrero, de medidas tributarias, administrativas y financieras de la Comunidad Autónoma de Extremadura. | 5 | as first published, then each change: 12 February 2015 to 30 November 2022 | 2025-12-19 |
| `ley-2015-004/` | Ley 4/2015, de 26 de febrero, de regulación del proceso de transición entre gobiernos en la Comunidad Autónoma de Extremadura. | 2 | as first published, then each change: 28 February 2015 to 14 March 2026 | 2026-04-20 |
| `ley-2015-006/` | Ley 6/2015, de 24 de marzo, Agraria de Extremadura. | 13 | as first published, then each change: 26 June 2015 to 9 September 2026 | 2026-10-30 |
| `ley-2015-007/` | Ley 7/2015, de 31 de marzo, por la que se regula el Estatuto de Capitalidad de la Ciudad de Mérida. | 1 | as first published: 8 April 2015 | 2025-12-19 |
| `ley-2015-008/` | Ley 8/2015, de 31 de marzo, de creación del Colegio Profesional de Técnicos Superiores en Laboratorio Clínico y Biomédico. | 1 | as first published: 27 April 2015 | 2025-12-19 |
| `ley-2015-009/` | Ley 9/2015, de 31 de marzo, por la que se regula la figura y funciones de los Cronistas Oficiales de Extremadura. | 2 | as first published, then each change: 7 April 2015 to 14 December 2016 | 2025-12-19 |
| `ley-2015-011/` | Ley 11/2015, de 8 de abril, de Autoridad de profesionales del Sistema Sanitario Público y centros sociosanitarios de Extremadura. | 1 | as first published: 11 April 2015 | 2025-12-19 |
| `ley-2015-012/` | Ley 12/2015, de 8 de abril, de igualdad social de lesbianas, gais, bisexuales, transexuales, transgénero e intersexuales y de políticas públicas contra la discriminación por orientación sexual e identidad de género en la Comunidad Autónoma de Extremadura. | 1 | as first published: 11 April 2015 | 2025-12-19 |
| `ley-2015-013/` | Ley 13/2015, de 8 de abril, de Función Pública de Extremadura. | 10 | as first published, then each change: 10 April 2015 to 27 June 2025 | 2025-12-19 |
| `ley-2015-014/` | Ley 14/2015, de 9 de abril, de Servicios Sociales de Extremadura. | 2 | as first published, then each change: 4 May 2015 to 1 January 2019 | 2025-12-19 |
| `ley-2015-015/` | Ley 15/2015, de 16 de abril, por la que se ordena el ejercicio de las profesiones del deporte en Extremadura. | 2 | as first published, then each change: 21 October 2015 to 15 December 2016 | 2025-12-19 |
| `ley-2015-016/` | Ley 16/2015, de 23 de abril, de protección ambiental de la Comunidad Autónoma de Extremadura. | 6 | as first published, then each change: 29 June 2015 to 23 September 2025 | 2026-01-12 |
| `ley-2015-018/` | Ley 18/2015, de 23 de diciembre, de cuentas abiertas para la Administración Pública Extremeña. | 1 | as first published: 30 December 2015 | 2025-12-19 |
| `ley-2015-019/` | Ley 19/2015, de 23 de diciembre, por la que se deroga la Ley 16/2001, de 14 de diciembre, reguladora del Consejo Consultivo de Extremadura. | 3 | as first published, then each change: 1 January 2016 to 26 May 2021 | 2025-12-19 |
| `decreto-ley-2016-001/` | Decreto-ley 1/2016, de 10 de mayo, de medidas extraordinarias contra la exclusión social. | 1 | as first published: 11 May 2016 | 2025-12-19 |
| `ley-2016-007/` | Ley 7/2016, de 21 de julio, de medidas extraordinarias contra la exclusión social. | 4 | as first published, then each change: 22 July 2016 to 26 June 2019 | 2025-12-19 |
| `ley-2017-002/` | Ley 2/2017, de 17 de febrero, de emergencia social de la vivienda de Extremadura. | 6 | as first published, then each change: 14 March 2017 to 31 March 2023 | 2025-12-19 |
| `ley-2017-006/` | Ley 6/2017, de 10 de julio, del Plan de Estadística de Extremadura 2017-2020. | 1 | as first published: 12 July 2017 | 2025-12-19 |
| `ley-2017-007/` | Ley 7/2017, de 1 de agosto, de Coordinación de Policías Locales de Extremadura. | 2 | as first published, then each change: 24 August 2017 to 18 October 2019 | 2025-12-19 |
| `ley-2018-002/` | Ley 2/2018, de 14 de febrero, de coordinación intersectorial y de simplificación de los procedimientos urbanísticos y de ordenación del territorio de Extremadura. | 4 | as first published, then each change: 16 May 2018 to 5 August 2026 | 2026-09-18 |
| `ley-2018-003/` | Ley 3/2018, de 21 de febrero, de Cámaras Oficiales de Comercio, Industria y Servicios de la Comunidad Autónoma de Extremadura. | 4 | as first published, then each change: 24 February 2018 to 5 August 2026 | 2026-09-18 |
| `decreto-legislativo-2018-001/` | Decreto Legislativo 1/2018, de 10 de abril, por el que se aprueba el texto refundido de las disposiciones legales de la Comunidad Autónoma de Extremadura en materia de tributos cedidos por el Estado. | 18 | as first published, then each change: 24 May 2018 to 5 August 2026 | 2026-08-17 |
| `ley-2018-005/` | Ley 5/2018, de 3 de mayo, de prevención del consumo de bebidas alcohólicas en la infancia y la adolescencia. | 1 | as first published: 8 November 2018 | 2025-12-20 |
| `ley-2018-007/` | Ley 7/2018, de 2 de agosto, extremeña de grandes instalaciones de ocio (LEGIO). | 3 | as first published, then each change: 6 August 2018 to 25 May 2020 | 2025-12-20 |
| `ley-2018-008/` | Ley 8/2018, de 23 de octubre, del comercio ambulante de Extremadura. | 4 | as first published, then each change: 27 October 2018 to 5 August 2026 | 2026-09-18 |
| `ley-2018-009/` | Ley 9/2018, de 30 de octubre, de sociedades cooperativas de Extremadura. | 5 | as first published, then each change: 3 November 2018 to 5 June 2024 | 2025-12-20 |
| `ley-2018-010/` | Ley 10/2018, de 22 de noviembre, del Tercer Sector Social de Extremadura. | 1 | as first published: 28 November 2018 | 2025-12-20 |
| `decreto-ley-2018-002/` | Decreto-ley 2/2018, de 11 de diciembre, de medidas urgentes para el restablecimiento de los derechos del personal al servicio de la Administración de la Junta de Extremadura en las situaciones de incapacidad temporal, y por el que se extienden las mejoras voluntarias de la acción protectora de la Seguridad Social a las situaciones de maternidad, paternidad, riesgo durante el embarazo y riesgo durante la lactancia. | 1 | as first published: 12 December 2018 | 2026-08-03 |
| `ley-2018-011/` | Ley 11/2018, de 21 de diciembre, de ordenación territorial y urbanística sostenible de Extremadura. | 9 | as first published, then each change: 27 June 2019 to 5 August 2026 | 2026-09-18 |
| `ley-2018-012/` | Ley 12/2018, de 26 de diciembre, de contratación pública socialmente responsable de Extremadura. | 6 | as first published, then each change: 1 January 2019 to 30 November 2022 | 2025-12-20 |
| `ley-2018-013/` | Ley 13/2018, de 26 de diciembre, de conciertos sociales para la prestación de servicios a las personas en los ámbitos social, sanitario y sociosanitario en Extremadura. | 2 | as first published, then each change: 1 January 2019 to 30 November 2022 | 2025-12-20 |
| `ley-2019-001/` | Ley 1/2019, de 21 de enero, de memoria histórica y democrática de Extremadura. | 3 | as first published, then each change: 24 July 2019 to 21 September 2026 | 2026-09-21 |
| `ley-2019-003/` | Ley 3/2019, de 22 de enero, de garantía de la autonomía municipal de Extremadura. | 2 | as first published, then each change: 29 January 2019 to 9 March 2021 | 2025-12-20 |
| `ley-2019-004/` | Ley 4/2019, de 18 de febrero, de mejora de la eficiencia energética y las condiciones térmicas y ambientales de los centros educativos extremeños. | 1 | as first published: 1 January 2019 | 2025-12-20 |
| `ley-2019-005/` | Ley 5/2019, de 20 de febrero, de Renta Extremeña Garantizada. | 2 | as first published, then each change: 26 June 2019 to 30 November 2022 | 2025-12-20 |
| `ley-2019-006/` | Ley 6/2019, de 20 de febrero, del Estatuto de las personas consumidoras de Extremadura. | 3 | as first published, then each change: 27 February 2019 to 30 November 2022 | 2025-12-20 |
| `ley-2019-007/` | Ley 7/2019, de 5 de abril, de espectáculos públicos y actividades recreativas de la Comunidad Autónoma de Extremadura. | 4 | as first published, then each change: 10 April 2019 to 30 November 2022 | 2025-12-20 |
| `ley-2019-008/` | Ley 8/2019, de 5 de abril, para una Administración más ágil en la Comunidad Autónoma de Extremadura. | 2 | as first published, then each change: 9 May 2019 to 30 November 2022 | 2025-12-20 |
| `ley-2019-010/` | Ley 10/2019, de 11 de abril, de protección civil y de gestión de emergencias de la Comunidad Autónoma de Extremadura. | 2 | as first published, then each change: 18 October 2019 to 30 November 2022 | 2025-12-20 |
| `ley-2019-011/` | Ley 11/2019, de 11 de abril, de promoción y acceso a la vivienda de Extremadura. | 5 | as first published, then each change: 7 May 2019 to 1 January 2024 | 2025-12-20 |
| `ley-2019-012/` | Ley 12/2019, de 11 de octubre, del Voluntariado de Extremadura. | 1 | as first published: 16 October 2019 | 2025-12-20 |
| `ley-2020-002/` | Ley 2/2020, de 4 de marzo, de apoyo, asistencia y reconocimiento a las víctimas de terrorismo de la Comunidad Autónoma de Extremadura. | 2 | as first published, then each change: 10 March 2020 to 30 November 2022 | 2025-12-20 |
| `decreto-ley-2020-001/` | Decreto-ley 1/2020, de 18 de marzo, por el que se establecen medidas liberalizadoras de los horarios de apertura de las actividades comerciales habilitadas por el Real Decreto 463/2020, de 14 de marzo, por el que se declara el estado de alarma para la gestión de la situación de crisis sanitaria ocasionado por el COVID-19. | 1 | as first published: 21 March 2020 | 2026-04-15 |
| `decreto-ley-2020-002/` | Decreto-ley 2/2020, de 25 de marzo, de medidas urgentes de carácter tributario para paliar los efectos del COVID-19 en la Comunidad Autónoma de Extremadura. | 2 | as first published, then each change: 27 March 2020 to 2 June 2020 | 2025-12-20 |
| `decreto-ley-2020-003/` | Decreto-ley 3/2020, de 25 de marzo, por el que se aprueban medidas urgentes y extraordinarias en el ámbito administrativo para responder al impacto de la crisis ocasionada por el COVID-19. | 1 | as first published: 27 March 2020 | 2025-12-20 |
| `decreto-ley-2020-004/` | Decreto-ley 4/2020, de 1 de abril, por el que se adoptan medidas urgentes y extraordinarias en el ámbito de la contratación pública para responder al impacto de la crisis ocasionada por el COVID-19. | 2 | as first published, then each change: 2 April 2020 to 27 April 2020 | 2025-12-20 |
| `decreto-ley-2020-005/` | Decreto-ley 5/2020, de 3 de abril, por el que se aprueban medidas urgentes y extraordinarias en materia de política social y sanitaria. | 2 | as first published, then each change: 6 April 2020 to 30 November 2022 | 2025-12-20 |
| `decreto-ley-2020-006/` | Decreto-ley 6/2020, de 17 de abril, de medidas extraordinarias y urgentes para la tramitación de las bases reguladoras y normativa específica de subvenciones, la ejecución de determinadas prestaciones de contratos administrativos y la selección de personal temporal mediante bolsas de trabajo, como consecuencia de la crisis ocasionada por el COVID-19. | 1 | as first published: 20 April 2020 | 2025-12-20 |
| `decreto-ley-2020-007/` | Decreto-ley 7/2020, de 24 de abril, por el que se aprueban medidas urgentes en materia de educación, para paliar los efectos de la emergencia sanitaria provocada por el COVID-19. | 2 | as first published, then each change: 27 April 2020 to 30 November 2022 | 2026-02-24 |
| `decreto-ley-2020-008/` | Decreto-ley 8/2020, de 24 de abril, por el que se adoptan medidas urgentes y extraordinarias para el mantenimiento y recuperación del empleo frente a la crisis ocasionada por el COVID-19. | 2 | as first published, then each change: 12 May 2020 to 2 June 2020 | 2026-01-23 |
| `decreto-ley-2020-009/` | Decreto-ley 9/2020, de 8 de mayo, por el que se aprueba una subvención para refuerzo del sistema de garantías de Extremadura, se establecen ayudas financieras a autónomos y empresas, y se adoptan medidas en materia de espectáculos públicos y actividades recreativas y de patrimonio histórico y cultural, para afrontar los efectos negativos del COVID-19. | 3 | as first published, then each change: 13 May 2020 to 16 June 2021 | 2025-12-20 |
| `decreto-ley-2020-010/` | Decreto-ley 10/2020, de 22 de mayo, de medidas urgentes para la reactivación económica en materia de edificación y ordenación del territorio destinadas a dinamizar el tejido económico y social de Extremadura, para afrontar los efectos negativos de la COVID-19. | 1 | as first published: 25 May 2020 | 2025-12-20 |
| `decreto-ley-2020-011/` | Decreto-ley 11/2020, de 29 de mayo, de medidas urgentes complementarias en materia tributaria para responder al impacto económico del COVID-19 en la Comunidad Autónoma de Extremadura y otras medidas adicionales. | 1 | as first published: 2 June 2020 | 2026-02-06 |
| `decreto-ley-2020-012/` | Decreto-ley 12/2020, de 19 de junio, de medidas extraordinarias y urgentes para la reactivación de la actividad económica y social en la Comunidad Autónoma de Extremadura en el proceso hacia la "Nueva Normalidad". | 4 | as first published, then each change: 20 June 2020 to 30 November 2022 | 2026-02-03 |
| `decreto-ley-2020-014/` | Decreto-ley 14/2020, de 22 de julio, de medidas para la activación de la demanda en la Comunidad Autónoma de Extremadura tras la crisis sanitaria. | 1 | as first published: 28 July 2020 | 2025-12-20 |
| `ley-2020-003/` | Ley 3/2020, de 29 de octubre, del sistema de préstamo de los libros de texto de Extremadura. | 1 | as first published: 5 November 2020 | 2025-12-20 |
| `ley-2020-005/` | Ley 5/2020, de 1 de diciembre, de Instituciones Museísticas de Extremadura. | 1 | as first published: 4 December 2020 | 2026-02-23 |
| `ley-2020-006/` | Ley 6/2020, de 1 de diciembre, de Artes Escénicas de Extremadura. | 1 | as first published: 4 December 2020 | 2026-02-23 |
| `decreto-ley-2021-003/` | Decreto-ley 3/2021, de 3 de marzo, de medidas urgentes para la modernización de la Administración Pública y para la ejecución del Plan de Recuperación, Transformación y Resiliencia. | 3 | as first published, then each change: 9 March 2021 to 5 June 2024 | 2025-12-20 |
| `ley-2021-002/` | Ley 2/2021, de 21 de mayo, de defensa, asistencia jurídica y comparecencia en juicio de la administración de la Comunidad Autónoma de Extremadura. | 1 | as first published: 26 May 2021 | 2025-12-20 |
| `decreto-ley-2021-004/` | Decreto-ley 4/2021, de 4 de junio, por el que se adoptan medidas de extraordinaria y urgente necesidad orientadas a establecer la prestación a la demanda y garantizar el equilibrio económico de los servicios de transporte público regular de uso general de viajeros por carretera sometidos a obligaciones de servicio público, en el contexto actual de crisis sanitaria y sus efectos en el ámbito de la movilidad de las personas, así como a impulsar la autonomía local en materia de comercio ambulante. | 1 | as first published: 9 June 2021 | 2025-12-20 |
| `decreto-ley-2021-005/` | Decreto-ley 5/2021, de 9 de junio, por el que se regulan y establecen ayudas directas a autónomos y empresas, financiadas por el Gobierno de España; se establecen las bases reguladoras de ayudas urgentes en el marco del desarrollo del plan corresponsables; se modifica el Decreto-ley 9/2020, de 8 de mayo, por el que se aprueba una subvención para refuerzo del sistema de garantías de Extremadura, se establecen ayudas financieras a autónomos y empresas, y se adoptan medidas en materia de espectáculos públicos y actividades recreativas y de patrimonio histórico y cultural, para afrontar los efectos negativos del COVID-19 y se modifica la Ley 3/2018, de 21 de febrero, de Cámaras Oficiales de Comercio, Industria y Servicios de Extremadura. | 3 | oldest version available, then each change: 16 June 2021 to 12 March 2022 | 2025-12-20 |
| `decreto-ley-2022-001/` | Decreto-ley 1/2022, de 2 de marzo, de medidas urgentes de mejora de la calidad en la contratación pública para la reactivación económica. | 4 | as first published, then each change: 8 March 2022 to 1 January 2023 | 2025-12-20 |
| `ley-2022-003/` | Ley 3/2022, de 17 de marzo, de medidas ante el reto demográfico y territorial de Extremadura. | 2 | as first published, then each change: 22 March 2022 to 30 November 2022 | 2025-12-20 |
| `ley-2022-002/` | Ley 2/2022, de 1 de abril, de bibliotecas de Extremadura. | 1 | as first published: 6 April 2022 | 2025-12-20 |
| `decreto-ley-2022-002/` | Decreto-ley 2/2022, de 4 de mayo, por el que se regula la actuación de la Junta de Extremadura y se establecen medidas urgentes en respuesta a los desplazamientos de personas por razones humanitarias a causa de la guerra en Ucrania, medidas urgentes de contratación pública y medidas fiscales. | 1 | as first published: 17 May 2022 | 2025-12-20 |
| `ley-2022-004/` | Ley 4/2022, de 27 de julio, de racionalización y simplificación administrativa de Extremadura. | 3 | as first published, then each change: 29 July 2022 to 29 January 2023 | 2025-12-20 |
| `ley-2022-005/` | Ley 5/2022, de 25 de noviembre, de medidas de mejora de los procesos de respuesta administrativa a la ciudadanía y para la prestación útil de los servicios públicos. | 2 | as first published, then each change: 30 November 2022 to 4 July 2026 | 2026-07-13 |
| `ley-2023-001/` | Ley 1/2023, de 2 de marzo, de gestión y ciclo urbano del agua de Extremadura. | 1 | as first published: 7 March 2023 | 2025-12-20 |
| `decreto-ley-2023-002/` | Decreto-ley 2/2023, de 8 de marzo, de medidas urgentes de impulso a la inteligencia artificial en Extremadura. | 1 | as first published: 11 March 2023 | 2025-12-20 |
| `ley-2023-002/` | Ley 2/2023, de 22 de marzo, por la que se regulan determinados aspectos de la Red ecológica europea Natura 2000 en la Comunidad Autónoma de Extremadura. | 1 | as first published: 24 March 2023 | 2025-12-20 |
| `ley-2023-003/` | Ley 3/2023, de 29 de marzo, de Cooperación y Solidaridad Internacional de Extremadura. | 1 | as first published: 1 April 2023 | 2025-12-20 |
| `ley-2024-002/` | Ley 2/2024, de 12 de abril, para la aplicación al municipio de Badajoz del régimen de organización de municipios de gran población. | 1 | as first published: 18 April 2024 | 2025-12-20 |
| `ley-2025-004/` | Ley 4/2025, de 15 de octubre, de Concordia de Extremadura. | 2 | as first published, then each change: 18 October 2025 to 21 September 2026 | 2026-09-21 |
| `decreto-ley-2026-004/` | Decreto-ley 4/2026, de 28 de julio, de actuaciones urgentes en materia de urbanismo para la agilización de la aprobación del planeamiento y su ejecución para el impulso a la promoción de vivienda. | 1 | as first published: 5 August 2026 | 2026-09-18 |
| `ley-1984-004/` | Ley 4/1984, de 27 de diciembre, de Ferias y Mercados de la Comunidad Autónoma de Extremadura. | 4 | as first published, then each change: 20 February 1985 to 26 June 2015; **repealed** 26 June 2015 by Ley 6/2015, de 24 de marzo (BOE-A-2015-4102) | 2025-12-16 |
| `ley-1985-008/` | Ley 8/1985, de 26 de noviembre, de Comparecencia en Juicio de la Junta de Extremadura. | 2 | as first published, then each change: 3 December 1985 to 26 May 2021; **repealed** 26 May 2021 by Ley 2/2021, de 21 de mayo (BOE-A-2021-10592) | 2025-12-17 |
| `ley-1990-001/` | Ley 1/1990, de 26 de abril, de Coordinación de Policías Locales de Extremadura. | 7 | as first published, then each change: 1 June 1990 to 24 August 2017; **repealed** 24 August 2017 by Ley 7/2017, de 1 de agosto (BOE-A-2017-10455) | 2025-12-17 |
| `ley-1997-006/` | Ley 6/1997, de 29 de mayo, de Bibliotecas de Extremadura. | 2 | as first published, then each change: 18 July 1997 to 6 April 2022; **repealed** 6 April 2022 by Ley 2/2022, de 1 de abril (BOE-A-2022-5854) | 2025-12-18 |
| `ley-1998-002/` | Ley 2/1998, de 26 de marzo, de Sociedades Cooperativas de Extremadura. | 5 | as first published, then each change: 2 July 1998 to 2 January 2019; **repealed** 2 January 2019 by Ley 9/2018, de 30 de octubre (BOE-A-2018-16345) | 2025-12-18 |
| `ley-2001-003/` | Ley 3/2001, de 26 de abril, de la Calidad, Promoción y Acceso a la Vivienda de Extremadura. | 6 | as first published, then each change: 29 August 2001 to 7 May 2019; **repealed** 7 May 2019 by Ley 11/2019, de 11 de abril (BOE-A-2019-7224) | 2025-12-18 |
| `ley-2001-006/` | Ley 6/2001, de 24 de mayo, del Estatuto de los Consumidores de Extremadura. | 7 | as first published, then each change: 13 July 2001 to 27 February 2019; **repealed** 27 February 2019 by Ley 6/2019, de 20 de febrero (BOE-A-2019-3492) | 2025-12-18 |
| `ley-2001-015/` | Ley 15/2001, de 14 de diciembre, del Suelo y Ordenación Territorial de Extremadura. | 14 | as first published, then each change: 23 January 2002 to 27 June 2019; **repealed** 27 June 2019 by Ley 11/2018, de 21 de diciembre (BOE-A-2019-1790) | 2025-12-18 |
| `ley-2001-017/` | Ley 17/2001, de 14 de diciembre, de Cámaras Oficiales de Comercio e Industria de la Comunidad Autónoma de Extremadura. | 2 | as first published, then each change: 23 January 2002 to 24 February 2018; **repealed** 24 February 2018 by Ley 3/2018, de 21 de febrero (BOE-A-2018-3361) | 2025-12-18 |
| `ley-2002-006/` | Ley 6/2002, de 27 de junio, de medidas de apoyo en materia de autopromoción de viviendas, accesibilidad y suelo. | 2 | as first published, then each change: 24 July 2002 to 7 May 2019; **repealed** 7 May 2019 by Ley 11/2019, de 11 de abril (BOE-A-2019-7224) | 2025-12-18 |
| `ley-2003-001/` | Ley 1/2003, de 27 de febrero, de Cooperación para el Desarrollo. | 3 | as first published, then each change: 19 March 2003 to 1 April 2023; **repealed** 1 April 2023 by Ley 3/2023, de 29 de marzo (BOE-A-2023-9097) | 2025-12-18 |
| `ley-2003-002/` | Ley 2/2003, de 13 de marzo, de la convivencia y el ocio de Extremadura. | 3 | as first published, then each change: 23 March 2003 to 8 November 2018; **repealed** 8 November 2018 by Ley 5/2018, de 3 de mayo (BOE-A-2018-6941) | 2025-12-18 |
| `ley-2004-001/` | Ley 1/2004, de 19 de febrero, de creación de la Empresa Pública "Gestión de Infraestructuras, Suelo y Vivienda de Extremadura". | 2 | as first published, then each change: 7 March 2004 to 4 February 2020; **repealed** 4 February 2020 by Ley 1/2020, de 31 de enero (BOE-A-2020-2458) | 2025-12-18 |
| `ley-2009-007/` | Ley 7/2009, de 17 de diciembre, de enajenación de viviendas de la Comunidad Autónoma de Extremadura. | 3 | as first published, then each change: 11 January 2010 to 7 May 2019; **repealed** 7 May 2019 by Ley 11/2019, de 11 de abril (BOE-A-2019-7224) | 2025-12-19 |
| `ley-2016-004/` | Ley 4/2016, de 6 de mayo, para el establecimiento de un régimen sancionador en materia de espectáculos públicos y actividades recreativas en la Comunidad Autónoma de Extremadura. | 2 | as first published, then each change: 9 May 2016 to 10 April 2019; **repealed** 10 April 2019 by Ley 7/2019, de 5 de abril (BOE-A-2019-7220) | 2025-12-19 |

## Source

The consolidated legislation of the Agencia Estatal Boletín Oficial del Estado (BOE), through its open-data API, <https://www.boe.es/datosabiertos/api/legislacion-consolidada>. For each consolidated norm it gives every block of the text (article, disposition, annex, heading) with every version of that block, the day each version took effect (fecha_vigencia) and the norm that made it (id_norma). Each version here is the whole text as it stood on one of those days. The last column above is the BOE's own last-update date for the consolidated text.

## Dates

- Each commit is dated at **noon, Europe/Madrid, on the day the change took effect**: the fecha_vigencia the BOE gives the new block versions.
- A day on which the BOE records a new block version that changes no words is not a version here.
- Block versions with no in-force date (the BOE's 99999999, a date not yet fixed) are left out.
- An act's first commit is its first publication when the BOE's earliest text is the act as enacted; otherwise it is the oldest version the BOE holds.
- Versions that take effect after the retrieval day are on the `futuro` branch, never merged into `main`.

## Files

`<act>/art-005.md` is Artículo 5, `art-005-bis.md` Artículo 5 bis; `da-01.md` the Disposición adicional primera, `dt-` transitional, `dd-` repealing and `df-` final dispositions (`-unica` for "única"); `preambulo.md` the preamble, `firma.md` the signature, `anexo-*.md` the annexes. The book, title, chapter and section headings sit at the top of the file of the article that follows them. One paragraph per line; a table one line per row, cells separated by ` | `.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the BOE's own text of that day, rebuilt from the source XML by a separate reader, and every file's text appears in it.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the norm that changed the text (a law, a decree-law, a ruling of the Constitutional Court), named by its title and BOE identifier, with an e-mail address that cannot exist (`<boe id>@boe.es.invalid`). The committer is always Lexifina.

## Limits

This is not an official publication. Only the texts published in the official journals are authentic. The history starts with the oldest text the BOE consolidates for each norm. Only the norms listed above are included; norms the BOE does not consolidate are not.
