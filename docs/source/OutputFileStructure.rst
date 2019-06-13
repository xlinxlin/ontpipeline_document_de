Die Struktur der Ausgabedaten
=============================

::

    Output_Directory/
     ├── Analysis_{Zeitstempel}/
     |    ├── Basecalled/
     |    ├── Barcodes/
     |    |    ├── barcode01/
     |    |    ├── barcode02/
     |    |    ├── barcode03/
     |    |    ├── unclassified/
     |    |    ├── Präfix01.fastq
     |    |    ├── Präfix02.fastq
     |    |    └── Präfix03.fastq
     |    ├── AdaperTrimmedFiles/
     |    |    ├── Präfix01_trimmed.fastq
     |    |    ├── Präfix02_trimmed.fastq
     |    |    └── Präfix03_trimmed.fastq
     |    ├── FiltedFiles/
     |    |    ├── Präfix01_filted.fastq
     |    |    ├── Präfix02_filted.fastq
     |    |    └── Präfix03_filted.fastq
     |    ├── StatFiles/
     |    |    ├── Präfix01_trimmed_stat.txt
     |    |    ├── Präfix02_trimmed_stat.txt
     |    |    ├── Präfix03_trimmed_stat.txt
     |    |    ├── Präfix01_filted_stat.txt
     |    |    ├── Präfix02_filted_stat.txt
     |    |    └── Präfix03_filted_stat.txt
     |    ├── Präfix01_Assembly/
     |    |    ├── ...
     |    |    └── assembly.fasta
     |    ├── Präfix02_Assembly/
     |    |    ├── ...
     |    |    └── assembly.fasta
     |    ├── Präfix03_Assembly/
     |    |    ├── ...
     |    |    └── assembly.fasta
     |    ├── Präfix01_Polishing/
     |    |    ├── run_Präfix01_busco/
     |    |    |    ├── ...
     |    |    |    └── full_table_Präfix01_busco.tsv
     |    |    ├── ...   
     |    |    └── pilon_1.fasta
     |    ├── Präfix02_Polishing/
     |    |    ├── run_Präfix02_busco/
     |    |    |    ├── ...
     |    |    |    └── full_table_Präfix02_busco.tsv
     |    |    ├── ...   
     |    |    └── pilon_1.fasta
     |    ├── Präfix03_Polishing/
     |    |    ├── run_Präfix03_busco/
     |    |    |    ├── ...
     |    |    |    └── full_table_Präfix03_busco.tsv
     |    |    ├── ...   
     |    |    └── pilon_1.fasta
     |    └── Logs/
     |         ├── guppy_basecaller.log
     |         ├── guppy_barcoder.log
     |         ├── Präfix01_trimmed.log
     |         ├── Präfix02_trimmed.log
     |         ├── Präfix03_trimmed.log
     |         ├── Präfix01_filted.log
     |         ├── Präfix02_filted.log
     |         ├── Präfix03_filted.log
     |         ├── Präfix01_assembly.log
     |         ├── Präfix02_assembly.log
     |         ├── Präfix03_assembly.log
     |         ├── Präfix01_polishing_1.log
     |         ├── Präfix02_polishing_1.log
     |         ├── Präfix03_polishing_1.log
     |         ├── Präfix01_busco.log
     |         ├── Präfix02_busco.log
     |         └── Präfix03_busco.log
     ├── pipelineWithLoop_{Zeitstempel}.pbs # Übermittelte PBS-Datei.
     └── userlog_{Zeitstempel}.log # Vom Benutzer angegebene Parameter.
     
    /home/{$USER}/
     ├── Ont_Pipeline.e* # Fehlermeldungen in dem Lauf. 
     └── Ont_Pipeline.o* # Nachrichten in dem Lauf.
     
    /opt/ontpipeline/logs/
     ├── ...
     └── {$USER}_error.log # Fehlermeldungen für das Java-Programm.
   