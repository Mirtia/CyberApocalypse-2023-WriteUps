# Last Hope

## Description

The quantum data came back and analyzed. DISASTER! Our best scientists all agree: Unfortunately our species and our whole culture are about to be eliminated. Due to abnormal behavior of the black hole's singularity our planet is about to get swallowed. Project "ONESHOT" is our last hope...

## Solution

We are given a `quantum_artifact.qasm` file, which contains language for describing quantum circuits. For some reason, an already existent python package that works with OpenQASM slipped my mind, so I imported the file to [IBM platform](https://cloud.ibm.com/catalog/services/qiskit-runtime) and run the program. I exported the results and examined the information.

```
...
success":true,
    "results":[
       {
          "shots":1,
          "success":true,
          "data":{
             "counts":{
                "0x4854427b615f676c316d7073335f30665f683070337d":1
             }
          },
          "meas_level":2,
          "header":{
             "clbit_label
...
```

Finally, I took the *counts* hex sequence and converted it to ASCII.

## Flag

```
HTB{a_gl1mps3_0f_h0p3}
```