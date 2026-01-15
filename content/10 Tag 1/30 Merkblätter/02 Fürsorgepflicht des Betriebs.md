---
{"publish":true,"created":"2026-01-15T08:54:02.886+01:00","modified":"2025-11-13T05:24:16.000+01:00","cssclasses":""}
---

## Das Wichtigste in Kürze

<iframe src="https://aburossi.github.io/prezi/BBK/merkblaetter/#/" style="border:0px #ffffff none;" name="myiFrame" scrolling="yes" frameborder="1" marginheight="0px" marginwidth="0px" height="550px" width="100%" allowfullscreen></iframe>

[Präsentation in einem neuen Fenster öffnen](https://aburossi.github.io/prezi/BBK/merkblaetter)

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
