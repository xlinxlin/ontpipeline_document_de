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

Methode(Method) [1]_ (Erfordlich)
_________________________________
Eine Assember-Methode auszuwählen.

.. note::
  * Long-read-only assembly: mit der "Long-read-only assembly"-Methode werden nur die Nanopore-Reads zum Assembler gebracht.
  * Hybrid assembly: mir der "Hybrid assembly"-Methode werden Illumina-Reads und die Nanopore-Reads zum Assembler gebracht.
  * Standardwert: Hybrid assembly.

.. image:: /img/AdvancedAssemblySettings.png

VCF [1]_ (Optional)
___________________
Eine VCF Datei wird erstellt, falls diese Option ausgewählt ist.

.. note::
  * Standardwert: nicht ausgewählt.
  
.. [1] Unicycler https://github.com/rrwick/Unicycler