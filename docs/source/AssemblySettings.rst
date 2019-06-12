Assembly Einstellung
====================

.. image:: /img/AssemblySettings.png

Modus(Mode) [1]_ (Erfordlich)
_____________________________
Ein Assember-Modus auszuwählen.

.. note::
  * Conservative: im Konservative-Modus wird das Assembly mit der geringsten Vollständigkeit und dem kleinsten Fehler erstellt.
  * Normal: im Normal-Modus wird das Assembly mit mittlerer Vollständigkeit und mittlerem Fehler erstellt.
  * Bold: im Grob-Modus wird das Assembly mit der höchsten Vollständigkeit und dem größten Fehler erstellt.
  * Standardwert: Normal.

Method [1]_ (Required)
______________________
Choose an assembly method.

.. note::
  * Long-read-only assembly: Long-read-only assembly using only long reads.
  * Hybrid assembly: Hybrid assembly using both Illumina reads and long reads. 
  * Default: Hybrid assembly.

.. image:: /img/AdvancedAssemblySettings.png

VCF [1]_ (Optional)
___________________
Produce a VCF by mapping the short reads to the final assembly if selected.

.. note::
  * Default: not selected.
  
.. [1] Unicycler https://github.com/rrwick/Unicycler