---
{"publish":true,"created":"2025-11-03T13:59:29.340+01:00","modified":"2025-11-13T05:21:20.211+01:00","cssclasses":""}
---

## Auftrag

>[!note] Überfliegen Sie die Seiten 252-254 im Handbuch. Merken Sie sich die vier Merkmale eines positiven Vorbilds. Besprechen Sie in Ihrer Gruppe die folgenden Reflexionsfragen und halten Sie Ihre Ergebnisse auf dem Pinboard fest.
> 
>> [!Question] Reflexionsfragen
>> **Positives Vorbild:**
>> - Wie können Sie im Berufsalltag als **positives Vorbild** für Ihre Lernenden agieren?
>> **Coaching-Methoden:**
>> - Mit welchen **konkreten Methoden** können Sie Ihre Lernenden im Sinne des **Coachings** unterstützen?
>> **Massgebender Führungsstil:**
>> - Was zeichnet einen **massgebenden Führungsstil** in der Berufsausbildung aus?
>> **Herausforderungen und Lösungen:**
>> - Welche **Herausforderungen** sehen Sie in Bezug auf die drei Ansätze und wie könnten Sie diese **meistern**?

Auf dem Pinboard finden Sie **[vier beschriftete Bereiche](https://tools.fobizz.com/pinboard/public_boards/d08684f4-97a1-4bce-9c79-772c0b01a871?token=919642dc5532154ffb797cf06da1c76b)**, die den Reflexionsfragen entsprechen. **Halten Sie die Ergebnisse Ihrer Gruppendiskussion in diesen Bereichen fest**. Erstellen Sie eine neue Karte in der jeweiligen Bereich, um Ihre **wichtigsten Gedanken und Ideen** zu notieren.

>[!bug]- [Pinboard](https://app.fobizz.com/pinboard/public_boards/d08684f4-97a1-4bce-9c79-772c0b01a871?embed=true&token=919642dc5532154ffb797cf06da1c76b)

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
