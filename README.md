# sbvs.mmp9
<p>
  A computer program works in the command line interface (CLI) to predict whether a compound is a potentially potent MMP9 inhibitor.
The program works on a machine running Ubuntu 22.04.3 LTS and with AutoDock Vina v1.2.3 (https://autodock-vina.readthedocs.io/en/latest/index.html) and PyPLIF HIPPOS v0.2.0 (https://github.com/radifar/PyPLIF-HIPPOS/releases/tag/0.2.0) installed.
</p>
<p>
  This computer program is an output of a research project funded by the Directorate of Research, Technology, and Community Services, the Directorate General of Higher Education, Research, and Technology, the Indonesian Ministry of Education, Culture, Research, and Technology (Contract No. 107/E5/PG.02.00.PL/2024).
</p>
<p>
  Installation: (i) Download the program into a suitable machine; (ii) Make the files sbvs.mmp9, ensplif.mmp9, and dectree.mmp9 executable with the chmod command; (iii) Copy the whole directory pyplif_hippos from the PyPLIF HIPPOS software to this program's "source" directory.  </p>
<p>
  Usage: Copy the tested compound(s) in the pdbqt format into the directory of this program, and then run the program by typing "./sbvs.mmp9 [file-name-of-the-compound-without-the-extension]" in the CLI. For example, the file CHEMBL4854379.pdbqt (https://www.ebi.ac.uk/chembl/compound_report_card/CHEMBL4854379/) is provided here. By typing "./sbvs.mmp9 CHEMBL4854379" in the CLI and pressing the Enter key, the compound CHEMBL4854379 will be run to predict its activity for about one and a half minutes. 
</p>
<p>
  Advanced usage: Basically, the sbvs.mmp9 command runs the commands ensplif.mmp9 and dectree.mmp9, subsequently. Therefore, to optimize computer power using parallel software (https://www.gnu.org/software/parallel/), predicting several compounds at once is highly recommended. This can be done by running in parallel the ensplif.mmp9 program and then run the dectree.mmp9 in parallel.  
</p>
