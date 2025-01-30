research_shell_ShinaMin
================
Shina Min
2025-01-29

### **Investigating the Gene-Cohort Interaction Between FTO and BMI**

Understanding the genetic and environmental determinants of **obesity**
is crucial for effective public health interventions. This research
explores **the FTO gene**, a key genetic determinant of **body mass
index (BMI)**, to assess whether its influence differs across birth
cohorts. It examines whether individuals born after World War II (WWII),
who were exposed to a higher-calorie diet, show a stronger genetic
**effect of FTO on BMI** compared to those born before WWII. To manage
large-scale multiomic datasets, this study employs **Linux-based tools**
and high-performance **cluster computing** for data preprocessing and
analysis.

### 1. Study Design and Data Collection

This study leverages **multiomic datasets** from 5,000 individuals
across 500 families in the United States and Denmark. These datasets
include **genomic, epigenomic, transcriptomic, proteomic, metabolomic,
and lipidomic profiles.** Families have been followed for over a decade,
allowing the integration of **whole-genome sequencing and lipid
profiling** to examine how FTO variants influence lipid metabolism and
BMI. Given the dataset’s complexity, cluster-based parallel computing is
used for preprocessing and efficient data management.

| Cohort_Group             | Key_Characteristics                                |
|:-------------------------|:---------------------------------------------------|
| Born Before WWII (≤1945) | Limited food availability, lower calorie intake    |
| Born After WWII (\>1945) | Industrialized food systems, higher calorie intake |

Comparison of Pre-WWII and Post-WWII Cohorts

### 2. Computational Analysis

Principal component analysis (PCA) is applied to lipidomic data to
identify biomarkers associated with obesity. Longitudinal statistical
modeling assesses whether FTO has a stronger effect on BMI in post-WWII
cohorts. Linux shell scripting and cluster-based processing ensure
computational efficiency for handling large datasets.

### Conclusion

This study clarifies the **gene-environment interaction** between **FTO
and BMI**, providing insights into obesity risk. By using
high-performance computing, it supports **precision medicine
strategies** for targeted interventions.

## **Shell Command Questions and My Solutions:**

After working through these shell commands, I documented the most
efficient solutions for each problem based on my understanding and
testing in a Linux environment.

### 1. Listing all files in the current directory, including hidden ones

To display all files, including hidden ones (which start with a `.`), I
used: `sh ls -la`

### 2. Finding the number of lines in a file named data.txt

To count the number of lines in data.txt, I used: `wc -l data.txt`, this
command outputs the total line count, which was helpful for verifying
dataset sizes before processing.

### 3. Searching for the string “error” in all .log files in the current directory

To identify occurrences of “error” across multiple log files, I ran:
`grep "error".log`, This scanned all `.log` files and returned only the
lines containing the keyword, making debugging easier.

### 4. Changing the permissions of a file named script.sh to make it executable

Since `script.sh` needed execution rights, I used: `chmod +x script.sh`,
running `ls -l script.sh` afterward confirmed the change by displaying x
(execute) permissions.

### 5. Displaying the last 20 lines of a file named output.log

To quickly check the most recent entries in `output.log`, I
used:`tail -n 20 output.log`. This command was useful for monitoring
logs in real-time.

### 6. Combining file1.txt and file2.txt into a new file named combined.txt

To merge two text files into a single file while preserving order, I
used: `cat file1.txt file2.txt > combined.txt`. Running
`cat combined.txt` verified that all contents were correctly appended.

### 7. Checking for the presence of the word “Completed” in status.txt and displaying the line

To filter `status.txt` and display lines containing “Completed”, I used:
`grep "Completed" status.txt`. This helped verify the completion of
certain processes in the file.

### 8. Sorting the lines in unsorted.txt in alphabetical order and saving to sorted.txt

To sort unsorted.txt alphabetically and save the output, I used:
`sort unsorted.txt > sorted.txt`. Afterward, running cat sorted.txt
confirmed that the file was correctly sorted.
