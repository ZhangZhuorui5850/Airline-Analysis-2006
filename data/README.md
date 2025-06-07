# Data Usage Instructions

The full airline dataset for 2006 is too large (~600MB) to include in this GitHub repository.

Therefore, follow the steps below to reproduce the analysis:

---

## Step 1: Transfer CSV to Linux system
Use **WinSCP** or any SCP tool to upload `2006.csv` to your Linux virtual machine.
Example local path:  
`C:\Users\yourname\Downloads\2006.csv`  
Example Linux destination:  
`/home/maria_dev/Assignment2/2006.csv`

---

## Step 2: Upload CSV to HDFS
If Ambari File View fails, use `putty` or terminal to run the following command:

```bash
hadoop fs -copyFromLocal /home/maria_dev/Assignment2/2006.csv /user/maria_dev/Assignment2/2006.csv
