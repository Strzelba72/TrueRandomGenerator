# TrueRandomGenerator
This GitHub project focuses on implementing a True Random Number Generator (TRNG) based on a scientific article titled "GPUs and chaos: a new true random number generator" by Je Sen Teh, Azman Samsudin, Mishal Al-Mazrooie, and Amir Akhavan. The project aims to reproduce and further develop the idea presented in the article using CPU threads as the computing platform.

The project leverages the principles of chaos theory(chaotic maps) to generate truly random numbers.

To determine the random values of the array X and R, I used the chaos maps that were left over
parallel triggered. This procedure allowed to obtain random values because,
there was a deliberate race for resources. To generate an 8-bit number
i needed 6 threads for chaos map and 6 threads for chaos maps and do functions
generating numbers along with post-processing.

Compiler:gcc (Rev6, Built by MSYS2 project) 13.1.0

Entropy per 100000 8-bit samples: 7.998

![alt text](https://github.com/Strzelba72/TrueRandomGenerator/blob/main/trng.png?raw=true)
