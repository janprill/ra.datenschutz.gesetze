# DSGVO

Hier findet Ihr die bisherigen Veröffentlichungen des Verordnung (EU) 2016/679 des Europäischen Parlaments und des Rates vom 27. April 2016 zum Schutz natürlicher Personen bei der Verarbeitung personenbezogener Daten, zum freien Datenverkehr und zur Aufhebung der Richtlinie 95/46/EG (Datenschutz-Grundverordnung - DSGVO).

Die Historie der Verordnung bis zu Ihrer aktuell gültigen, konsolidierten Fassung lässt sich in dieser Repository nachvollziehen. Die Historie ist wie folgt:

1. Verordnung (EU) 2016/679 des Europäischen Parlaments und des Rates vom 27. April 2016 zum Schutz natürlicher Personen bei der Verarbeitung personenbezogener Daten, zum freien Datenverkehr und zur Aufhebung der Richtlinie 95/46/EG (Datenschutz-Grundverordnung) (Text von Bedeutung für den EWR)
ABl. L 119 vom 4.5.2016, S. 1–88 (BG, ES, CS, DA, DE, ET, EL, EN, FR, GA, HR, IT, LV, LT, HU, MT, NL, PL, PT, RO, SK, SL, FI, SV) - Celex: 32016R0679
2. Berichtigung der Verordnung (EU) 2016/679 des Europäischen Parlaments und des Rates vom 27. April 2016 zum Schutz natürlicher Personen bei der Verarbeitung personenbezogener Daten, zum freien Datenverkehr und zur Aufhebung der Richtlinie 95/46/EG (ABl. L 119 vom 4.5.2016)
ABl. L 314 vom 22.11.2016, S. 72–72 (DE, ET, IT, HU), ELI: http://data.europa.eu/eli/reg/2016/679/corrigendum/2016-11-22/oj, Celex: 32016R0679R(01)
3. Berichtigung der Verordnung (EU) 2016/679 des Europäischen Parlaments und des Rates vom 27. April 2016 zum Schutz natürlicher Personen bei der Verarbeitung personenbezogener Daten, zum freien Datenverkehr und zur Aufhebung der Richtlinie 95/46/EG (Datenschutz-Grundverordnung) (ABl. L 119 vom 4.5.2016), ABl. L 127 vom 23.5.2018, S. 2–8 (DE), ELI: http://data.europa.eu/eli/reg/2016/679/corrigendum/2018-05-23/oj, Celex: 32016R0679R(02)

In dieser Repository findet Ihr jeweils die XML-Veröffentlichungen, sowie das konsolidierte, entsprechend der Berichtigungen angepasste XML. Dadurch lassen sich die Änderungen über das Versionskontrollsystem GIT leicht nachvollziehen. Ein paar Beispiele dafür liefere ich Euch unten.

Zunächst aber möchte ich ein Branching-Konzept für die Konsolidierung erarbeiten. Ich orientiere mich dabei (bisher) bewusst nicht an anderen Git-Repos, die sich mit der Konsolidierung von Gesetzen befassen, sondern möchte einen ersten, eigenen, unbelasteten Aufschlag wagen:

1. Im "master" findet sich eine konsolidierte, aktuell gültige Version des Gesetzes. Das macht für mich Sinn, weil dies der Text ist, an dem ein Nutzer der Repo regelmäßig Interesse haben dürfte. 
2. Ebenfalls im Master findet sich ein Verzeichnis "originals". Darin finden sich die XML-formattierten, aber ansonsten unberührten Texte, wie Sie in den Amtsblättern veröffentlicht worden sind. 
3. So wie in einem "develop"-Branch in der Softwareentwicklung pflege ich einen Branch "consolidation" darin wird die Konsolidierungsarbeit geleistet. Sobald eine Konsolidierung abgeschlossen ist, wird die Arbeit in "master" gemerged und als eine gültige Version, gleichsam ein "release" getaggt.

TODO: Beispiele