Reads Filter Einstellung
========================

.. image:: /img/ReadsFilterSettings.png

.. image:: /img/AdvancedReadsFilterSettings.png

Porechop Einstellung [1]_ (Optional)
____________________________________
Die Optionen für Porechop einzustellen.

.. note::
  * "I want to trim adapter" auszuwählen, wenn Sie Porechop verwenden möchten, um die Adapter der Sequenzen zu trimmen. Standardwert: ausgewählt.
  * "I want to skip splitting reads based on middle adapters" auszuwählen, wenn Sie keine Sequenz, die sich in der Mitte einen Adapter befindet, teilen möchten. Standardwert: nicht ausgewählt.

Read Score(Read Score) [2]_ (Erfordlich)
________________________________________
Einer durchschnittlichen Mindestwert für die Readqualität einzugeben, um die Reads zu filtern.

.. note::
  * Standardwert: 9. 

Readlänge(Read Length) [2] (Erfordlich)
_______________________________________
Eine minimale Readlänge einzugeben, um  die Reads zu filtern.

.. note::
  * Standardwert: 500.

Kopf trimmen(Head Crop) [2]_ (Erfordlich)
_________________________________________
Anzahl der Nukleotide, die ab dem Beginn des Reads geschnitten werden sollen, einzugeben.

.. note::
  * Standardwert: 50. 
 
.. [1] Porechop https://github.com/rrwick/Porechop
.. [2] NanoFilt https://github.com/wdecoster/nanofilt