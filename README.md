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
