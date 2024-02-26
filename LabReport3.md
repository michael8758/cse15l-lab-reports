# **Lab Report Three**
---
# **Part 1 - Bugs**

## Failure Inducing Input
```
public void testReverseInPlaceFailure() {
    int[] input = {1, 2, 3, 4, 5};
    ArrayExamples.reverseInPlace(input);
    assertArrayEquals(new int[]{5, 4, 3, 2, 1}, input);
}
```

## Non-Failure Inducing Input
```
public void testReverseInPlaceFailure() {
    int[] input = {1, 2, 3, 4, 5};
    ArrayExamples.reverseInPlace(input);
    assertArrayEquals(new int[]{5, 4, 3, 4, 5}, input);
}
```

## Symptom
<img width="782" alt="Screenshot 2024-02-11 at 3 01 46 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/306c2b85-caba-4f1c-a80c-ccf5ddc26f11">

## Fixing the Bug
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
        arr[i] = arr[arr.length - i - 1];
    }
}
```

```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length / 2; i += 1) {
        int temp = arr[i];
        arr[i] = arr[arr.length - i - 1];
        arr[arr.length - i - 1] = temp;
    }
}
```

This fix addresses the issue because the original code does not use a temporary variable to hold a value during the process of the reversal. Further, it also incorrectly interates through the array, because it iterates through the entire array and in doing so, it leads to the elements returning to their original positions. The code that fixes this array creates a variable `temp` to store the value of the element during the reveresal process, which allows the reversal process to execeute without losing any data in the values. Further, by setting the iteration to only half the length of the array, it is ensured that there the elements are only swapped once and they do not go back to their original positions.

-----

# **Part 2 - Researching Commands**
## **Command: `find`**

### `-type` option

```find ./technical -type d```

```
./technical
./technical/government
./technical/government/About_LSC
./technical/government/Env_Prot_Agen
./technical/government/Alcohol_Problems
./technical/government/Gen_Account_Office
./technical/government/Post_Rate_Comm
./technical/government/Media
./technical/plos
./technical/biomed
./technical/911report
```

```find ./technical -type f```

```
./technical/plos/pmed.0020239.txt
./technical/plos/journal.pbio.0020241.txt
./technical/plos/pmed.0020005.txt
./technical/plos/journal.pbio.0020043.txt
./technical/plos/pmed.0020039.txt
./technical/plos/pmed.0010071.txt
./technical/plos/journal.pbio.0030127.txt
./technical/plos/pmed.0010058.txt
./technical/plos/pmed.0010070.txt
./technical/plos/pmed.0010064.txt
./technical/plos/pmed.0020158.txt
./technical/plos/journal.pbio.0020042.txt
./technical/plos/journal.pbio.0020297.txt
./technical/plos/pmed.0020206.txt
./technical/plos/pmed.0020212.txt
./technical/plos/pmed.0020216.txt
./technical/plos/journal.pbio.0030094.txt
./technical/plos/journal.pbio.0020046.txt
./technical/plos/pmed.0020028.txt
./technical/plos/journal.pbio.0020052.txt
./technical/plos/pmed.0020148.txt
./technical/plos/pmed.0020160.txt
./technical/plos/pmed.0010048.txt
./technical/plos/pmed.0010060.txt
./technical/plos/journal.pbio.0030137.txt
./technical/plos/journal.pbio.0030136.txt
./technical/plos/pmed.0010061.txt
./technical/plos/pmed.0010049.txt
./technical/plos/pmed.0020161.txt
```

The `-type` option for the `find` class specifies the type of file or directory that is being found. In the examples above, type `f` stands for file, and type `d` stands for directory.

-----
### `-name` option

```find ./technical -name "biomed"```

``` ./technical/biomed```


```find ./technical -name "*.txt"```


```./technical/plos/pmed.0020239.txt
./technical/plos/journal.pbio.0020241.txt
./technical/plos/pmed.0020005.txt
./technical/plos/journal.pbio.0020043.txt
./technical/plos/pmed.0020039.txt
./technical/plos/pmed.0010071.txt
./technical/plos/journal.pbio.0030127.txt
./technical/plos/pmed.0010058.txt
./technical/plos/pmed.0010070.txt
./technical/plos/pmed.0010064.txt
./technical/plos/pmed.0020158.txt
./technical/plos/journal.pbio.0020042.txt
./technical/plos/journal.pbio.0020297.txt
./technical/plos/pmed.0020206.txt
./technical/plos/pmed.0020212.txt
./technical/plos/pmed.0020216.txt
./technical/plos/journal.pbio.0030094.txt
./technical/plos/journal.pbio.0020046.txt
./technical/plos/pmed.0020028.txt
./technical/plos/journal.pbio.0020052.txt
./technical/plos/pmed.0020148.txt
```

The `-name` option for the `find` class searches for files or directories based on the specified name. In the examples provided above, I used an example where I searched for a directory with the `biomed` keyword contained in it, and I also used `*.txt` to search for all files that contain the keyword `.txt`.

------
### `-size` option

```find ./technical -size +200k```

```./technical/government/About_LSC/commission_report.txt
./technical/government/Env_Prot_Agen/bill.txt
./technical/government/Gen_Account_Office/GovernmentAuditingStandards_yb2002ed.txt
./technical/government/Gen_Account_Office/Statements_Feb28-1997_volume.txt
./technical/government/Gen_Account_Office/d01591sp.txt
./technical/911report/chapter-13.4.txt
./technical/911report/chapter-13.5.txt
./technical/911report/chapter-3.txt
```


```find ./technical -size -50k```

```./technical
./technical/government
./technical/government/About_LSC
./technical/government/Env_Prot_Agen
./technical/government/Alcohol_Problems
./technical/government/Post_Rate_Comm
./technical/plos/pmed.0020191.txt
./technical/plos/pmed.0020226.txt
./technical/911report
```

The `-size' option for the `find` class searches for files that are above or below a certain size, where k - kibibytes, M - mebibytes, G - gibitypes. In the examples I provided above, I searched for all files in the technical directory that are greater than 200 kilobytes, and also in the second example, I searched for files in the technical directory that are less than 50 kilobytes.

---
### Sources Used

https://man7.org/linux/man-pages/man1/find.1.html - (searched on google "find command-line options")
