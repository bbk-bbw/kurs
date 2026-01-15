---
{"publish":true,"created":"2025-11-03T13:59:29.228+01:00","modified":"2026-01-15T08:01:18.551+01:00","cssclasses":""}
---

### Auftrag - Lebenskurven

> [!abstract] In diesem Auftrag nehmen Sie sich Zeit, um Ihre **eigene Lebenskurve allgemein und in Bezug auf Ihre Ausbildung** zu formulieren und zu reflektieren. 
> - Sie analysieren **prägende Erfahrungen und Ereignisse** in Ihrem Leben. 
> - Sie überlegen, welche **Faktoren und Strategien** Ihnen geholfen haben, *resilient* zu bleiben, 
> - Sie reflektieren über Ihre Werte und Ziele und wie Sie diese umgesetzt haben.

#### Ablauf

>[!abstract] Schritt 1. **Einzelarbeit (10 Minuten):**
 - Sie erhalten [[20 Tag 2/10 Eigenheiten junger Erwachsener/Lebenskurven\|zwei Grafiken]] und zeichnen Sie darauf Ihre **persönliche Lebenskurve** sowie Ihre **Lebenskurve in der Ausbildung**.
 - Markieren Sie besondere **Erfahrungen und Ereignisse** (Höhen- und Tiefpunkte), die für Sie prägend waren.
   
>[!abstract] Schritt 2. **Partnerarbeit (10 Minuten):**
 - Finden Sie sich zu zweit zusammen.
 - Erklären Sie Ihrem/Ihrer Partner/in Ihre Kurven.
 - Beantworten Sie sich gegenseitig die folgenden drei Fragen. Beziehen Sie sich dabei **spezifisch auf die Höhenpunkte und Tiefpunkte** Ihrer Kurven:
     - **Welche Faktoren und Strategien** haben Ihnen geholfen, resilient zu bleiben oder haben Sie beeinträchtigt?
     - **Welche Werte und Ziele** waren Ihnen (in diesen Momenten) wichtig und wie haben Sie sie umgesetzt?
     - **Wie sind Sie mit den Herausforderungen** (Tiefpunkten) oder Erfolgen (Höhepunkten) umgegangen?
            
>[!abstract] Schritt 3. **Austausch im Plenum (10 Minuten):**
 - Diskussion über Gemeinsamkeiten und Unterschiede in den persönlichen Erfahrungen.
        

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
