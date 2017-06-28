# CodeStat

A tool for quantifying the parallelization effort

CodeStat is a tool that can be used to quantify the programming effort required to parallelize a code. It takes as input a configuration file and the source code. The configuration file contains a list of valid file extensions (such as, .c, .cpp, .cu, .cl, ...), and a list of framework specific method calls, or compiler directives (such as, #pragma omp, proc_bind, or omp_set_num_threads in OpenMP). 

CodeStat analyzes the code by looking for framework specific code-statements provided in the configuration file, and provides as output the total number of lines of code (LOC) and the number of LOC written in OpenMP, OpenCL, OpenACC, or CUDA. 

The configuration files for OpenMP, OpenCL, OpenACC, and CUDA are provided by CodeStat. Other programming frameworks can be supported by simply creating a new configuration file and adding the framework specific code-statements to the list. The list of statements for a given programming language is usually provided in the corresponding documentation or reference guides. 

The tool itself and instructions on how to use it will be available soon. 
