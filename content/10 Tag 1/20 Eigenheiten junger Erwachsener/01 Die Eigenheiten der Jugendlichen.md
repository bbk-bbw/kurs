---
{"publish":true,"created":"2025-11-03T13:59:29.220+01:00","modified":"2025-11-13T05:22:03.137+01:00","cssclasses":""}
---

## Eigenheiten der 15- bis 20-Jährigen Lernenden

>[!abstract] Einführung
>
>* Jugendliche zwischen 15 und 20 Jahren befinden sich in einer **Phase des Umbruchs**: Sie sind weder Kind noch Erwachsener.
>* Diese **Adoleszenz** ist geprägt von **körperlichen und psychischen Veränderungen**, der Suche nach der eigenen Identität und dem Wunsch nach Unabhängigkeit.
>* Als Berufsbildner spielen Sie eine wichtige Rolle in dieser Entwicklungsphase und können die Lernenden durch **Verständnis, klare Regeln und gezielte Förderung** unterstützen.
>
>>[!question] Adoleszenz: Herausforderungen und Chancen im Berufsalltag
>>
>>Die [[Ressourcen/Glossar/Adoleszenz]] ist eine **spannende, aber auch herausfordernde Zeit**, sowohl für die Jugendlichen selbst als auch für ihr Umfeld.  Diskutieren Sie in Ihrer Gruppe die folgenden Fragen:
>>* Welche **typischen Verhaltensweisen** von Jugendlichen in diesem Alter sind Ihnen im (Berufs-)Alltag begegnet?
>>* Welche **Chancen** bietet diese Entwicklungsphase für die Ausbildung?
>>* Wo sehen Sie die grössten **Herausforderungen**?


> [!success] Lernziele
>In diesem Modul beschäftigen wir uns mit den **Eigenheiten der 15- bis 20-jährigen Lernenden**. Wir betrachten die **physischen und psychischen Veränderungen** in der Adoleszenz, die damit verbundenen **Herausforderungen** und wie Sie als Berufsbildner die Lernenden in dieser Phase optimal begleiten können. Das Ziel dieses Moduls ist, dass…
>* Sie die **Entwicklungsphase der Adoleszenz** verstehen und die Bedürfnisse der Lernenden erkennen.
>* Sie **Strategien entwickeln**, um Jugendliche in diesem Alter optimal zu fördern und zu unterstützen.
>* Sie **sicher im Umgang mit herausfordernden Situationen** im Berufsalltag sind.

---


<iframe src="https://aburossi.github.io/prezi/BBK/eigenheiten/#/" style="border:0px #ffffff none;" name="myiFrame" scrolling="no" frameborder="1" marginheight="0px" marginwidth="0px" height="550px" width="100%" allowfullscreen></iframe>

[Präsentation in einem neuen Fenster öffnen](https://aburossi.github.io/prezi/BBK/eigenheiten)

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

