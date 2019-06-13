Allgemein Einstelllung
======================

.. image:: /img/GeneralSettings.png

ONT Verzeichnis(ONT Dir.) (Erfordlich)
______________________________________
Der Verzeichnispfad zu den Nanopore-Reads einzugeben.

.. note::
  * **Beispiel:** :file:`/path/to/your/ONT/reads/directory`
  
ONT Verzeichnis(Illumina Dir.) (Optional/Erfordlich)
____________________________________________________
Der Verzeichnispfad zu den Illumina-Reads einzugeben.

.. note::
  * **Beispiel:** :file:`/path/to/your/Illumina/reads/directory`
  * Erfordlich wenn "hybrid-assembly" oder/und "polishing" ausgewählt wird/werden.

Ausgabeverzeichnis(Output Dir.) (Erfordlich)
____________________________________________
Der Verzeichnispfad zu den Ausgaben einzugeben.

.. note::
  * **Beispiel:** :file:`/path/to/your/output/directory`

Musterblatt(Sample sheet) (Optional)
____________________________________
Der Pfadname zum Musterblatt einzugeben.

.. note::
  * Das Dateiformat des Musterblattes muss CSV oder TSV sein.

.. warning::
  * Unterstrich('_') ist im Probenname **nicht** erlaubt.
  
Präfix(Prefix) (Optional)
_________________________
Ein Präfix für die Umbenennung der Nanopore-Reads nach "demultiplexing" einzugeben.

.. note::
  * **Bespiel:** ID .
  * Standardwert: barcode .

(Theads)Threads (Erfordlich)
____________________________
Die benötige Anzahl der Threads/CPUs für den Pipeline-Lauf einzugeben.

.. note::
  * Standardwert: 8.

(Barcodes)Barcodes (Optional)
_____________________________
Welche Barcodes, die zum Pipeline-Lauf gebracht werden, einzugeben. Einfach die Barcode-Nummern, die mit dem Komma getrennt werden, einzugeben. 

.. note::
  * **Beispiel:** 1,2,3,4
  * Falls alle Barcodes zum Pipeline-Lauf gebracht werden, einfach dieses Feld leer lassen.