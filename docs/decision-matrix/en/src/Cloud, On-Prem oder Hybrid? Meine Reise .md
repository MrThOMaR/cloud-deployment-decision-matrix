Cloud, On-Prem oder Hybrid? Meine Reise zu einer strukturierten Entscheidung

Als ich vor ein paar Jahren mit meinen damaligen Kollegen @Michael Sinn und @Ullrich Dreyer die Flux MES gründeten, stellte sich mir kurz darauf immer wieder die Frage, wo man seine Anwendung betreiben sollte und warum. Da wir unser MES cloud-native entwickelten, war klar, dass es irgendwie in die Cloud musste. Aber auch da hat man mehrere Optionen, wo diese Cloud liegt. Die verschiedenen Meinungen von Stakeholdern waren in dieser Hinsicht nicht immer hilfreich.

#Der Investor
Alles muss in "die" Cloud, sonst skaliert euer Business nicht.

#Der Kunde
Was nicht bei mir auf dem Server läuft, dem traue ich nicht.

In diesem Spannungsfeld bekam ich meine erste nützliche Orientierung über einen Mentor aus dem Bereich Operations, der mir über unseren Accelerator, die @NCA, zur Seite gestellt wurde. Er vermittelte mir, dass man als Start-up gar keine andere Wahl hätte, als Public Cloud Infrastruktur zu nutzen. Man hätte weder das Geld noch das Personal, um eigene Infrastruktur aufzubauen. Wenn aber die Public Cloud Kosten ein bestimmtes Maß überschreiten, dann sollte man prüfen, ob der Aufbau und der eigene Betrieb der Infrastruktur nicht wieder kostengünstiger in einem z.B. angemieteten Space in einem RZ wäre. Als erste Orientierung war diese Aussage schon sehr hilfreich. Mich hat nach und nach interessiert, ob solche Entscheidungen, vor allem wenn man nicht im Start-up Umfeld ist, auch qualitativ und quantitativ getroffen werden können.
Mit dem Verlassen des Start-ups ist dieser Gedankengang in den Hintergrund gerückt und ich habe mich nicht weiter damit beschäftigt. Vor einigen Monaten aber regte mein Software**-**Architekt an, dass wir für ein neues Produkt die Entscheidung über die grundlegende Software Architektur anhand von Qualitätsanforderungen ableiten sollten. Hierbei kam das Architecture Styles Worksheet (https://developertoarchitect.com/downloads/worksheets.html) von @Marc Richards zum Einsatz. Diese Form der Entscheidungsmatrix, bei der man über die Kriterien zum Architektur-Stil kommt, hat mein früheres Interesse wiederbelebt. Ich fragte mich nun, gibt es sowas auch für die Entscheidung, wie ich eine Anwendung betreiben sollte?

Bei meiner Recherche habe ich sehr viele, auch nützliche, Informationen gefunden. Aber keine Form, die das Thema so abstrahiert, wie das Worksheet von @Marc Richards. Aus diesem Grund beschloss ich im letzten Jahr, das "Worksheet" selbst zu entwickeln. Das Ergebnis ist eine Entscheidungsmatrix, die dem Leser hilft, anhand von Kriterien herauszufinden, welche Betriebsart wie gut zu seinen Ansprüchen passt. Das Ergebnis habe ich nun unter die Creative Commons Lizenz gestellt und möchte dieses teilen.

Um einen ersten Überblick zu bekommen, bietet euch die README.md (https://github.com/MrThOMaR/cloud-deployment-decision-matrix/blob/main/README.md) einen sehr guten Einstieg. Wer direkt mit der Entscheidungsmatrix starten möchte, findet sie hier: [docs/decision-matrix/en/src/decision-matrix.md](https://github.com/MrThOMaR/cloud-deployment-decision-matrix/blob/main/docs/decision-matrix/en/src/decision-matrix.md)

Bei Fragen schreibt mir eine Direktnachricht hier auf LinkedIn oder auch gerne über GitHub.