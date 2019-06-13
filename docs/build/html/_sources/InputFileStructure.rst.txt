Die Struktur der Eingabedaten
=============================
Start von Base Calling
______________________
Start die Pipeline von Base Calling.

::
   
    ONT_Reads_Directory/
    ├── HPz800_20180821_FAJ18422_MN17776_sequencing_run_VIM4_Janina_26844_read_11_ch_171_strand.fast5
    ├── HPz800_20180821_FAJ18422_MN17776_sequencing_run_VIM4_Janina_26844_read_11_ch_203_strand.fast5
    ├── HPz800_20180821_FAJ18422_MN17776_sequencing_run_VIM4_Janina_26844_read_15_ch_344_strand.fast5   
    ├── HPz800_20180821_FAJ18422_MN17776_sequencing_run_VIM4_Janina_26844_read_17_ch_249_strand.fast5
    ├── HPz800_20180821_FAJ18422_MN17776_sequencing_run_VIM4_Janina_26844_read_19_ch_397_strand.fast5
    └── ......
    
    Illumina_Reads_Directory/
    ├── Präfix01_HQ_1.fastq.gz
    ├── Präfix01_HQ_2.fastq.gz
    ├── Präfix02_HQ_1.fastq.gz
    ├── Präfix02_HQ_2.fastq.gz
    ├── Präfix03_HQ_1.fastq.gz
    ├── Präfix03_HQ_2.fastq.gz
    └── ......

.. note::
  * Die Benennungsregeln für jedes Illumina-Reads Paar: Präfix_HQ_1.fastq.gz  Präfix_HQ_2.fastq.gz
  * "Präfix" ist der Probenname und das ist identisch für jedes Paar.
  * "*" bedeuted beliebig lange Zeichen.
  
.. warning::
  * Unterstrich('_') ist im Präfix nicht erlaubt.

Start von Demultiplexing
________________________
Start die Pipeline von Demultiplexing.

::
   
    ONT_Reads_Directory/
    ├── fastq_runid_50a6171cadcfb6b5cb2dae4e75a0ccc05b71e3d8_0.fastq
    ├── fastq_runid_50a6171cadcfb6b5cb2dae4e75a0ccc05b71e3d8_1.fastq
    ├── fastq_runid_50a6171cadcfb6b5cb2dae4e75a0ccc05b71e3d8_2.fastq 
    ├── fastq_runid_50a6171cadcfb6b5cb2dae4e75a0ccc05b71e3d8_3.fastq
    ├── fastq_runid_50a6171cadcfb6b5cb2dae4e75a0ccc05b71e3d8_4.fastq
    └── ......
    
    Illumina_Reads_Directory/
    ├── Präfix01_HQ_1.fastq.gz
    ├── Präfix01_HQ_2.fastq.gz
    ├── Präfix02_HQ_1.fastq.gz
    ├── Präfix02_HQ_2.fastq.gz
    ├── Präfix03_HQ_1.fastq.gz
    ├── Präfix03_HQ_2.fastq.gz
    └── ......


Start von Reads Filter
______________________
Start die Pipeline von Reads Filter.

::

    ONT_Reads_Directory/
    ├── Präfix01.fastq
    ├── Präfix02.fastq
    ├── Präfix03.fastq 
    ├── Präfix04.fastq
    ├── Präfix05.fastq
    └── ......
    
    Illumina_Reads_Directory/
    ├── Präfix01_HQ_1.fastq.gz
    ├── Präfix01_HQ_2.fastq.gz
    ├── Präfix02_HQ_1.fastq.gz
    ├── Präfix02_HQ_2.fastq.gz
    ├── Präfix03_HQ_1.fastq.gz
    ├── Präfix03_HQ_2.fastq.gz
    └── ......

Start von Assembly
___________________
Start die Pipeline von Assembly.

::
   
    ONT_Reads_Directory/
    ├── Präfix01.fastq
    ├── Präfix02.fastq
    ├── Präfix03.fastq 
    ├── Präfix04.fastq
    ├── Präfix05.fastq
    └── ......
    
    Illumina_Reads_Directory/
    ├── Präfix01_HQ_1.fastq.gz
    ├── Präfix01_HQ_2.fastq.gz
    ├── Präfix02_HQ_1.fastq.gz
    ├── Präfix02_HQ_2.fastq.gz
    ├── Präfix03_HQ_1.fastq.gz
    ├── Präfix03_HQ_2.fastq.gz
    └── ......
    
Start von Polishing
___________________
Start die Pipeline von Polishing.

::
   
    ONT_Reads_Directory/
    ├── Präfix01.fasta
    ├── Präfix02.fasta
    ├── Präfix03.fasta 
    ├── Präfix04.fasta
    ├── Präfix05.fasta
    └── ......
    
    Illumina_Reads_Directory/
    ├── Präfix01_HQ_1.fastq.gz
    ├── Präfix01_HQ_2.fastq.gz
    ├── Präfix02_HQ_1.fastq.gz
    ├── Präfix02_HQ_2.fastq.gz
    ├── Präfix03_HQ_1.fastq.gz
    ├── Präfix03_HQ_2.fastq.gz
    └── ......

Musterblatt(Sample Sheet)
_________________________
.. csv-table:: Musterblatt
   :header: Probenname,Barcode
   :widths: 20, 20

   Probenname1,barcode01
   Probenname2,barcode02
   Probenname3,barcode03
   Probenname4,barcode04
   Probenname5,barcode05
   
.. note::
  * Das Dateiformat des Musterblattes ist entweder CSV (Trennzeichen ist das Komma) oder TSV (Trennzeichen ist die Tabulatortaste).
  * Die Benennungsregeln für Barcode: barcodeXX ("barcode" kann beliebig Zeichen sein, aber "XX" muss zweistellig sein,z.B. 01,02,03,...,10,11,12,...)