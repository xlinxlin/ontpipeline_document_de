Base Calling Einstellung
========================

.. image:: /img/BasecallingSettings.png

(Flowcell ID)Flowcell ID [2]_ (Erfordlich)
__________________________________________
Eine Flowcell-ID aus der Liste auszuwählen.

(Kit Nummer)Kit Number [2]_ (Erfordlich)
________________________________________
Eine Kit-Nummer aus der Liste auszuwählen.

.. image:: /img/AdvancedBasecallingSettings.png

(Modus)Mode (Erfordlich)
________________________
Guppy "Base Calling" Modus einzustellen.

.. note::
  * Standardwert: high-accuracy.
  
Gerät(Device) (Erfordlich)
__________________________
Das Sequenzier-Geräte einzustellen.

.. note::
  * Standardwert: PromethION.

cpu_threads_per_caller [1]_ (Standardwert)
__________________________________________

.. note::
  * Standardwert: 1.

records_per_fastq [2]_ (Standardwert)
_____________________________________
.. note::
  * Standardwert: 0.
  * Die Dateien werden per "Worker(CPU)" und per "Run ID" erstellt.

recursive [2]_ (Standardwert)
_____________________________
.. note::
  * Standardwert: die Eingabedateien werden rekursiv durchgesucht.


.. [1] Guppy v3.0.3 Release https://community.nanoporetech.com/posts/guppy-3-0-release
.. [2] How to configure Guppy parameters https://community.nanoporetech.com/protocols/Guppy-protocol-preRev/v/gpb_2003_v1_revg_14dec2018/how-to-configure-guppy-parameters