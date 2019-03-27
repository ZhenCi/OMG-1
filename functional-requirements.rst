Functional Requirements
=======================


Input
-----
    Validly submitted gene expression files are in the following format. It is a plain text file with three columns of TAB-separated(see annex for a complete example). The file contains an optional header line, followed by a reference to the expression of each gene in the sample(for example, Control Sample) and the processing sample(for example, KnockOutSample).
    *See the txt file pattern as following:*

    ===========  =================  =================
      gene_id      ControlSample      KnockOutSample
    ===========  =================  =================
     AT1G01010      1.198558083        2.036161827
     AT1G01020      13.75736234        13.370796 
     AT1G01030      0.833779536        0.203616183 
     AT1G01040      9.58846466         7.126566394 
     AT1G01046      0                  0 
     AT1G01050      23.81482799        21.10821094 
     AT1G01060      0.625334652        1.221697096 
     AT1G01070      1.719670292        0.950208853 
     AT1G01080      28.34850421        25.24840665 
     AT1G01090      58.26034505        42.96301455 
     AT1G01100      1066.508249        1308.030358 
     AT1G01110      2.709783491        1.425313279
    ===========  =================  =================


Output
----------------------
    The web application displays a **table** and a **scatter plot** when given a gene expression file.


Analyzing
~~~~~~~~~~~~~~~
    Web applications show a table and a scatter diagram giving a gene expression file. The table contains a list of differential expression genes in the following format:

    ===========  =================  =================  =============
      gene_id      control_sample    knockout_sample     log_2[FC]
    ===========  =================  =================  =============
     AT1G01010      1.198558083        2.036161827          0.76
    ===========  =================  =================  =============


 
Plot Analyzing
~~~~~~~~~~~~~~
    The scatter diagram shows the genes expressed differently. The x-axis is the 'Control' and the Y-axis is the 'KnockOut'. If provided in the upload file, replace Control and Cancel with the assigned column name.

    .. image:: /image/GED.png

