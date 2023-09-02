# bash scripting assingments
## wc_linux_code
silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/alkanes$ `wc -w -m *.pdb`
| 156 |1158 |cubane.pdb |
|-----|-----|-----------|
|  84 | 622 | ethane.pdb|
|  57 | 422 |methane.pdb|
| 246 |1828 |octane.pdb |
| 165 |1226 |pentane.pdb|
| 111 | 825 |propane.pdb|
| 819 |6081 |total      |

silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/alkanes$ `wc -w -m *.pdb >lengthsF.txt`

silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/alkanes$ `more lengthsF.txt`
| 156 |1158 |cubane.pdb |
|-----|-----|-----------|
|  84 | 622 |ethane.pdb |
|  57 | 422 |methane.pdb|
| 246 |1828 |octane.pdb |
| 165 |1226 |pentane.pdb|
| 111 | 825 |propane.pdb|
| 819 |6081 |total      |

silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/alkanes$

## pipe_linux_code
silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/alkanes$ `wc -l *.pdb`
 | 20| cubane.pdb |
 |---|------------|
 | 12| ethane.pdb |
 |  9| methane.pdb|
 | 30| octane.pdb |
 | 21| pentane.pdb|
 | 15| propane.pdb|
 |107| total      |
 
silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/alkanes$ `wc -l *.pdb | sort -n | head -n 3 >my_sortedOut.txt`

silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/alkanes$ `more my_sortedOut.txt`
 |9 | methane.pdb|
 |--|------------|
 |12| ethane.pdb |
 |15| propane.pdb|
 
silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/alkanes$
## cut_linux_code
silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/alkanes$ `cd ../`

silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data$ `cd animal-counts/`

silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/animal-counts$ `ls
animals.csv`

silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/animal-counts$ `cat animals.csv`
|2012-11-05,deer,5   |
|--------------------|
|2012-11-05,rabbit,22|
|2012-11-05,raccoon,7|
|2012-11-06,rabbit,19|
|2012-11-06,deer,2   |
|2012-11-06,fox,4    |
|2012-11-07,rabbit,16|
|2012-11-07,bear,1   |

silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/animal-counts$ `cut -d ',' -f 2 animals.csv`
|deer   |
|-------|
|rabbit |
|raccoon|
|rabbit |
|deer   |
|fox    |
|rabbit |
|bear   |

silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/animal-counts$ `cut -d '-' -f 1 animals.csv`
|2012|
|----|
|2012|
|2012|
|2012|
|2012|
|2012|
|2012|
|2012|

silantoi@DESKTOP-4CSCM70:~/shell-lesson-data/exercise-data/animal-counts$

