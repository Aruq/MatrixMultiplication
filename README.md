# MatrixMultiplication
Matrix Multiplication with MPI
A difficulty it was the spread of the data to the worker.
At first, the matrix dimensions will be broadcast via `MPI_Bcast(&matrix_properties, 4, MPI_INT, 0, MPI_COMM_WORLD);` to the workers.

The size of the matrices is fixed. Now the 2-Dim matrix is converted into a 1-Dim matrix. So it is easier and safer to distribute the matrix data.
