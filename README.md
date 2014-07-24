Murmur3
=======

Julia implementation of Murmur3 hashing.

##Performance
Tested on Windows 7 (64 bit) with Intel core i5 3570K at 4222.25 Mhz. Julia performance is measured relative to the reference C++ implementation performance.

| Payload | Iterations  | C++   | Julia x86 32-bit  | Julia x86 128-bit | Julia x64 128-bit |
| ------- | -----------:| -----:| -----------------:| -----------------:| -----------------:|
| 5   B   | 100,000,000 | 1.000 | **6.774** ± 0.019 | **5.668** ± 0.013 | **6.691** ± 0.007 |
| 15  B   | 50,000,000  | 1.000 | **5.580** ± 0.012 | **5.500** ± 0.003 | **5.580** ± 0.007 |
| 256 B   | 5,000,000   | 1.000 | **1.143** ± 0.002 | **1.496** ± 0.006 | **1.581** ± 0.002 |
| 256 KiB | 5,000       | 1.000 | **1.031** ± 0.001 | **1.263** ± 0.002 | **1.227** ± 0.003 |
| 256 MiB | 10          | 1.000 | **1.030** ± 0.003 | **1.257** ± 0.002 | **1.229** ± 0.004 |
