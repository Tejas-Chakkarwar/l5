# l5
HPC Practicals
For running openmp programs run commands:-
To execute: go to file path and open terminal and enter
g++ -fopenmp filename.cpp -o filename
hit enter and again type
./filename

To run CUDA programs on Collab, follow these steps:
Go to Google Collab
Create a new Notebook(.ipynb file).
Click on Runtime and change runtime type to GPU.
Now run !pip install git+https://github.com/afnan47/cuda.git in a cell.
On a new cell run %load_ext nvcc_plugin
Test the following code
%%cu
#include <iostream>
int main(){
  std::cout << "Hello World\n";
  return 0;
}
Remember to add %%cu before writing the C++ code for every CUDA program. CUDA is now set.
