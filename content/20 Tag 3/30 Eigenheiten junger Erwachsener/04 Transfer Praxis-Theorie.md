---
{"publish":true,"created":"2025-11-03T13:59:29.230+01:00","modified":"2025-11-13T05:23:34.365+01:00","cssclasses":""}
---

### Transfer Praxis-Theorie

>[!abstract] In den [[10 Tag 1/10 Rolle BerufsbildnerIn/03 Rollenspiel\|Rollenspiele]] haben Sie herausfordernde Situationen erlebt (Praxis) und sich mit den Grundlagen des Reifeprozesses (Kap. 5.1) auseinandergesetzt (Theorie).
>
> In diesem Auftrag verknüpfen wir nun Ihre praktischen Erfahrungen aus dem Rollenspiel mit den konkreten Handlungsempfehlungen aus dem Handbuch (Kap. 5.2) und schliessen mit einer persönlichen Reflexion ab.

>[!success] Lernziele
> Das Ziel des Auftrags ist, dass…
>
>   * ...Sie Ihre praktischen Erfahrungen aus dem Rollenspiel mit dem theoretischen Wissen aus dem Handbuch (Kap. 5.2) verknüpfen.
>   * ...Sie Ihr Handeln im Rollenspiel anhand von Fachtexten analysieren und alternative Handlungsstrategien ableiten.
>   * ...Sie persönliche Stärken und Entwicklungsfelder im Umgang mit Lernenden in der Adoleszenz identifizieren.

-----

#### 1\. Leseauftrag (Einzelarbeit)

>[!note] Lesen Sie **Kapitel 5.2: Umgang mit Lernenden in der Adoleszenz"** (S. 269–270) im Handbuch.
>
> Konzentrieren Sie sich beim Lesen besonders auf die **"Hinweise im Umgang mit verhaltensauffälligen Lernenden"** auf Seite 270. Überlegen Sie bereits beim Lesen, wie diese Tipps zu den von Ihnen erlebten Rollenspielen passen.

-----
#### 2\. Diskussionsauftrag (Gruppenarbeit)

* Finden Sie sich wieder in Ihren **ursprünglichen Rollenspiel-Gruppen** zusammen.
* Rufen Sie sich die von Ihnen gespielten Situationen (z.B. Zuspätkommen, Verweigerung von Aufgaben) und Ihre Notizen auf dem Pinboard in Erinnerung.

>[!question] Leitfrage für die Diskussion:
>
> Welche der **"Hinweise" aus Kapitel 5.2** hätten Ihnen in der Rolle des/der Berufsbildners/in in den gespielten Situationen **konkret geholfen**?
> 
>>[!tip] Hilfsfragen zur Vertiefung:
>>
>>   * **Zuspätkommen / Verweigerung (Situation 1 & 4):**
>>
>>       * Wie hätte der Hinweis **"Klare Grenzen setzen"** die Dynamik im Gespräch verändert?
>>       * Inwiefern war das Verhalten des/der Lernenden ein "Ausloten von Grenzen", wie es der Text beschreibt?
>>
>>   * **Konflikt mit Kollegen (Situation 3):**
>>
>>       * Welche Rolle spielte der Tipp **"Keine Schuldzuweisungen machen"** und **"Konflikte auf der Sachebene angehen"**?
>>       * Haben Sie intuitiv versucht, **"Interesse für die Situation und Werte"** des/der Lernenden zu zeigen?
>>
>>   * **Wiederholte Fehler (Situation 2):**
>>
>>       * Wie passt hier die **"Gratwanderung zwischen Schonen und Fordern"**?
>>       * Wie hätten Sie den Tipp **"Scheitern nicht vorwegnehmen"** und **"an die Möglichkeiten der Jugendlichen glauben"** anwenden können?
>>
>>   * **Allgemein:**
>>
>>       * Welche der "Tatsachen" von Seite 269 (z.B. "Hinter grossspurigem Verhalten verstecken sich oft Unsicherheiten", "Jugendliche suchen Sicherheit") konnten Sie im Rollenspiel beobachten?

-----

#### 3\. Persönliche Reflexion (Einzelarbeit)

>[!abstract] Auftrag: Persönliche Stärken und Entwicklungsfelder
>
> Beantworten Sie die beiden folgenden Fragen:
>
> 1.  **Persönliche Stärken:** Wo sehen Sie, basierend auf den Rollenspielen und der Theorie, Ihre persönlichen Stärken im Umgang mit jugendlichen Lernenden?
> 2.  **Entwicklungspotenzial:** Wo und wie möchten Sie sich in diesem Bereich gezielt verbessern oder weiterentwickeln?

>[!bug] Persönliche Reflexion

<iframe src="https://app.lumi.education/api/v1/run/gTlD9X/embed" width="1088" height="720" frameborder="0" allowfullscreen="allowfullscreen" allow="geolocation *; microphone *; camera *; midi *; encrypted-media *"></iframe><script src="https://app.Lumi.education/api/v1/h5p/core/js/h5p-resizer.js" charset="UTF-8"></script>

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

