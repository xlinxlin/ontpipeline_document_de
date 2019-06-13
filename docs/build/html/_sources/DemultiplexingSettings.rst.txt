Demultiplexing Einstellung
==========================

.. image:: /img/DemultiplexingSettings.png

Barcode Kit(Barcode kit) [1]_ (Optional)
________________________________________
Einer Barcode-Kit oder mehrere Barcode-Kits aus der List auszuwählen, falls der/die verwendet wird/werden.

.. note::
  * Falls keiner Barcode-Kit verwendet wird, einfach dieses Feld leer lassen.
  * Mehrfachauswahl ist möglich.
  
records_per_fastq [1]_ (Standardwert)
_____________________________________

.. note::
  * Standardwert: 0.
  * Die Dateien werden per "Worker(CPU)" und per "Run ID" erstellt.

recursive [1]_ (Standardwert)
______________________________

.. note::
  * Standardwert: die Eingabedateien werden rekursiv durchgesucht.
  
trim_barcodes [2]_ (Default)
____________________________

.. note::
  * Die Barcodes aus den Ausgabesequenzen in den FASTQ-Dateien werden geschnitten.

 
.. [1] How to configure Guppy parameters https://community.nanoporetech.com/protocols/Guppy-protocol-preRev/v/gpb_2003_v1_revg_14dec2018/how-to-configure-guppy-parameters
.. [2] Guppy update (v3.1.5) https://community.nanoporetech.com/posts/guppy-update-v3-1-5