---
{"publish":true,"created":"2026-01-15T08:54:02.891+01:00","modified":"2025-11-13T05:24:08.000+01:00","cssclasses":""}
---

## Merkblattreihe «Gleiche Chancen und korrekter Umgang»

>[!abstract] Einführung
>
>* **Chancengleichheit** ist ein Grundrecht und sollte in jedem Betrieb gelebt werden.
>* Ein **korrekter Umgang** und ein **Klima des Vertrauens** sind essentiell für eine erfolgreiche Ausbildung.
>* **Frühzeitiges Erkennen** und **angemessenes Reagieren** auf Probleme sind zentral.
>
>>[!question] Herausforderungen im Umgang mit Lernenden
>>
>>**Unterschiedliche Persönlichkeiten**, **persönliche Probleme** der Lernenden oder auch **Konflikte** im Team können die Ausbildungszeit erschweren.  
>>Tauschen Sie sich in Ihrer Gruppe über folgende Fragen aus und halten Sie die wichtigsten Punkte fest:
>>* Welche **Herausforderungen** sind Ihnen im **Umgang mit Lernenden** bereits begegnet?
>>* **Inwiefern** haben alle Lernenden die **gleichen Chancen in der Ausbildung**?
>>* Welche Bedeutung hat ein **respektvolles und faires Miteinander im Betrieb** für die Ausbildung?

> [!success] Lernziele
>In diesem Modul beschäftigen wir uns mit der Merkblattreihe «**Gleiche Chancen und korrekter Umgang**».  Diese bietet Ihnen wertvolle Informationen und Handlungsempfehlungen für den Umgang mit **Herausforderungen** in der Ausbildung. **Das Ziel dieses Moduls ist, dass…**
>* …Sie die wichtigsten **Themen** der Merkblattreihe kennen und deren **Relevanz** für die Ausbildung verstehen.
>* …Sie **Massnahmen** zur **Prävention** von **Chancenungleichheiten** und **Belästigungen** ableiten und im Berufsalltag umsetzen können.
>* …Sie wissen, wie Sie bei **Problemen** im Zusammenhang mit den Themen der Merkblattreihe **kompetent vorgehen** und **Lernende unterstützen** können.


---

```dataviewjs
const current = dv.current();
const folderParts = current.file.folder.split("/");
const folderName = folderParts.at(-1);
const trimmedFolderName = folderName.substring(3); // Remove "20 ", "30 ", etc.

dv.header(3, `Weiter im Modul ${trimmedFolderName}`);

const pages = dv.pages()
  .where(p =>
    p.file.folder === current.file.folder &&
    p.file.name > current.file.name &&
    p.file.path !== current.file.path &&
    p.publish === true // Only include notes with `publish: true` in frontmatter
  );

dv.list(
  pages.map(p =>
    dv.fileLink(p.file.path, false, p.file.name.substring(3)) // Trim filename display
  )
);


