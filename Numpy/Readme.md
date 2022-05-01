# NumPy Functions

## Magic Function

| Sr. No. | Command | Description                |
| ------- | ------- | -------------------------- |
| 1       | %time   | Time to complete a process |

## Array creation functions

| Sr. No. | Function   | Description                                                                                                                                                                  |
| ------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1       | array      | Convert input data (list, tuple, array, or other sequence type) to an ndarray either by inferring a dtype or explicitly specifying a dtype; copies the input data by default |
| 2       | asarray    | Convert input to ndarray, but do not copy if the input is already an ndarray                                                                                                 |
| 3       | arange     | Like the built-in range but returns an ndarray instead of a list                                                                                                             |
| 4       | ones       | Produce an array of all 1s with the given shape and dtype                                                                                                                    |
| 5       | ones_like  | takes another array and produces a ones array of the same shape and dtype                                                                                                    |
| 6       | zeros      | Produce an array of all 0s with the given shape and dtype                                                                                                                    |
| 7       | zeros_like | takes another array and produces a zeros array of the same shape and dtype                                                                                                   |
| 8       | empty      | Create new arrays by allocating new memory, but do not populate with any values like ones and zeros                                                                          |
| 9       | empty_like | Create new arrays by allocating new memory, but do not populate with any values like ones_like and zeros_like                                                                |
| 10      | full       | Produce an array of the given shape and dtype with all values set to the indicated “fill value”                                                                              |
| 11      | full_like  | full_like takes another array and produces a filled array of the same shape and dtype                                                                                        |
| 12      | eye        | identity Create a square N × N identity matrix (1s on the diagonal and 0s elsewhere)                                                                                         |

## NumPy data types

| Sr. No. | Function     | Description                        |
| ------- | ------------ | ---------------------------------- |
| 1       | random.randn | Random numbers in specific shape   |
| 2       | dtype        | Data type of the array             |
| 3       | ndim         | Dimension of the array             |
| 4       | shape        | Shape of the array                 |
| 5       | reshape      | Reshape the array to desired shape |

| Sr. No. | Data Type                         | Type Code    | Description                                                                                                            |
| ------- | --------------------------------- | ------------ | ---------------------------------------------------------------------------------------------------------------------- |
| 1       | int8, uint8                       | i1, u1       | Signed and unsigned 8-bit (1 byte) integer types                                                                       |
| 2       | int16, uint16                     | i2, u2       | Signed and unsigned 16-bit integer types                                                                               |
| 3       | int32, uint32                     | i4, u4       | Signed and unsigned 32-bit integer types                                                                               |
| 4       | int64, uint64                     | i8, u8       | Signed and unsigned 64-bit integer types                                                                               |
| 5       | float16                           | f2           | Half-precision oating point                                                                                            |
| 6       | float32                           | f4 or f      | Standard single-precision foating point; compatible with C foat                                                        |
| 7       | float64                           | f8 or d      | Standard double-precision foating point; compatible with C double and Python float object                              |
| 8       | float128                          | f16 or g     | Extended-precision foating point                                                                                       |
| 9       | complex64, complex128, complex256 | c8, c16, c32 | Complex numbers represented by two 32, 64, or 128 foats, respectively                                                  |
| 10      | bool                              | ?            | Boolean type storing True and False values                                                                             |
| 11      | object                            | O            | Python object type; a value can be any Python object                                                                   |
| 12      | string\_                          | S            | Fixed-length ASCII string type (1 byte per character); for example, to create a string dtype with length 10, use 'S10' |
| 13      | unicode\_                         | U            | Fixed-length Unicode type (number of bytes platform specific); same specification semantics as string\_ (e.g., 'U10')  |

## Arithmetic with NumPy Arrays

| Sr. No. | Operation | Description    |
| ------- | --------- | -------------- |
| 1       | +         | Addition       |
| 2       | -         | Subtraction    |
| 3       | \*        | Multiplication |
| 4       | /         | division       |
| 5       | > , <     | Comaprison     |
| 6       | \*\*      | Power          |

## Indexing and Slicing

- Basic indexing and slicing
- Indexing with slices
- Boolean Indexing
- Fancy indexing

| Sr. No. | Function  | Description            |
| ------- | --------- | ---------------------- |
| 1       | copy      | copy the arry          |
| 2       | T         | Transpose of the array |
| 3       | transpose | Transpose of the array |
| 4       | swapaxes  | swap given axes        |

## Universal Functions: Fast Element-Wise Array Functions

### Unary ufuncs

| Sr. No. | Function                                          | Description                                                                                                |
| ------- | ------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| 1       | abs, fabs                                         | Compute the absolute value element-wise for integer, floating-point, or complex values                     |
| 2       | sqrt                                              | Compute the square root of each element (equivalent to arr \*\* 0.5)                                       |
| 3       | square                                            | Compute the square of each element (equivalent to arr \*\* 2)                                              |
| 4       | exp                                               | Compute the exponent ex of each element                                                                    |
| 5       | log, log10, log2, log1p                           | Natural logarithm (base e), log base 10, log base 2, and log(1 + x), respectively                          |
| 6       | sign                                              | Compute the sign of each element: 1 (positive), 0 (zero), or –1 (negative)                                 |
| 7       | ceil                                              | Compute the ceiling of each element (i.e., the smallest integer greater than or equal to that number)      |
| 8       | floor                                             | Compute the floor of each element (i.e., the largest integer less than or equal to each element)           |
| 9       | rint                                              | Round elements to the nearest integer, preserving the dtype                                                |
| 10      | modf                                              | Return fractional and integral parts of array as a separate array                                          |
| 11      | isnan                                             | Return boolean array indicating whether each value is NaN (Not a Number)                                   |
| 12      | isfinite, isinf                                   | Return boolean array indicating whether each element is finite (non-inf, non-NaN) or infinite respectively |
| 13      | cos, cosh, sin, sinh, tan, tanh                   | Regular and hyperbolic trigonometric functions                                                             |
| 14      | arccos, arccosh, arcsin, arcsinh, arctan, arctanh | Inverse trigonometric functions                                                                            |
| 15      | logical_not                                       | Compute truth value of not x element-wise (equivalent to ~arr)                                             |

### Binary universal functions

| Sr. No. | Function                                                  | Description                                                                                                  |
| ------- | --------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| 1       | add                                                       | Add corresponding elements in arrays                                                                         |
| 2       | subtract                                                  | Subtract elements in second array from first array                                                           |
| 3       | multiply                                                  | Multiply array elements                                                                                      |
| 4       | divide, floor_divide                                      | Divide or floor divide (truncating the remainder)                                                            |
| 5       | power                                                     | Raise elements in first array to powers indicated in second array                                            |
| 6       | maximum, fmax                                             | Element-wise maximum; fmax ignores NaN                                                                       |
| 7       | minimum, fmin                                             | Element-wise minimum; fmin ignores NaN                                                                       |
| 8       | mod                                                       | Element-wise modulus (remainder of division)                                                                 |
|         |
| 9       | copysign                                                  | Copy sign of values in second argument to values in first argument                                           |
| 10      | greater, greater_equal,less, less_equal, equal, not_equal | Perform element-wise comparison, yielding boolean array (equivalent to infix operators >, >=, <, <=, ==, !=) |
| 11      | logical_and, logical_or, logical_xor                      | Compute element-wise truth value of logical operation                                                        |

## Array-Oriented Programming with Arrays

| Sr. No. | Function     | Description                                                                 |
| ------- | ------------ | --------------------------------------------------------------------------- |
| 1       | meshgrid     | takes two 1D arrays and produces two 2D matrices corresponding to all pairs |
| 2       | plt.imshow   | Show plot of the given data                                                 |
| 3       | plt.colorbar | Color Bar                                                                   |
| 4       | plt.title    | Title of the graph                                                          |

#### Expressing Conditional Logic as Array Operations

| Sr. No. | Function | Description           |
| ------- | -------- | --------------------- |
| 1       | where    | condotional statement |

#### Basic array statistical methods

| Sr. No. | Function       | Description                                                                                                        |
| ------- | -------------- | ------------------------------------------------------------------------------------------------------------------ |
| 1       | sum            | Sum of all the elements in the array or along an axis; zero-length arrays have sum 0                               |
| 2       | mean           | Arithmetic mean; zero-length arrays have NaN mean                                                                  |
| 3       | std, var       | Standard deviation and variance, respectively, with optional degrees of freedom adjustment (default denominator n) |
| 4       | min, max       | Minimum and maximum                                                                                                |
| 5       | argmin, argmax | Indices of minimum and maximum elements, respectively                                                              |
| 6       | cumsum         | Cumulative sum of elements starting from 0                                                                         |
| 7       | cumprod        | Cumulative product of elements starting from 1                                                                     |

#### Methods for Boolean Arrays

| Sr. No. | Function | Description        |
| ------- | -------- | ------------------ |
| 1       | any      | Any of the element |
| 2       | all      | all the elements   |
| 3       | sum      | Sum                |

#### Sorting

| Sr. No. | Function | Description             |
| ------- | -------- | ----------------------- |
| 1       | sort     | sorted copy of an array |

#### Unique and Other Set Logic

| Sr. No. | Function          | Description                                                                        |
| ------- | ----------------- | ---------------------------------------------------------------------------------- |
| 1       | unique(x)         | Compute the sorted, unique elements in x                                           |
| 2       | intersect1d(x, y) | Compute the sorted, common elements in x and y                                     |
| 3       | union1d(x, y)     | Compute the sorted union of elements                                               |
| 4       | in1d(x, y)        | Compute a boolean array indicating whether each element of x is contained in y     |
| 5       | setdiff1d(x, y)   | Set difference, elements in x that are not in y                                    |
| 6       | setxor1d(x, y)    | Set symmetric differences; elements that are in either of the arrays, but not both |

## File Input and Output with Arrays

| Sr. No. | Function         | Description                                     |
| ------- | ---------------- | ----------------------------------------------- |
| 1       | save             | saving array data on disk                       |
| 2       | load             | load‐ing array data on disk                     |
| 3       | savez            | save multiple arrays in an uncompressed archive |
| 4       | savez_compressed | save multiple arrays in an compressed archive   |

## Linear Algebra

| Sr. No. | Function | Description                                                                                                                                                |
| ------- | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1       | diag     | Return the diagonal (or off-diagonal) elements of a square matrix as a 1D array, or convert a 1D array into a square matrix with zeros on the off-diagonal |
| 2       | dot      | Matrix multiplication                                                                                                                                      |
| 3       | trace    | Compute the sum of the diagonal elements                                                                                                                   |
| 4       | det      | Compute the matrix determinant                                                                                                                             |
| 5       | eig      | Compute the eigenvalues and eigenvectors of a square matrix                                                                                                |
| 6       | inv      | Compute the inverse of a square matrix                                                                                                                     |
| 7       | pinv     | Compute the Moore-Penrose pseudo-inverse of a matrix                                                                                                       |
| 8       | qr       | Compute the QR decomposition                                                                                                                               |
| 9       | svd      | Compute the singular value decomposition (SVD)                                                                                                             |
| 10      | solve    | Solve the linear system Ax = b for x, where A is a square matrix                                                                                           |
| 11      | lstsq    | Compute the least-squares solution to Ax = b                                                                                                               |

## Pseudorandom Number Generation

| Sr. No. | Function    | Description                                                                                          |
| ------- | ----------- | ---------------------------------------------------------------------------------------------------- |
| 1       | seed        | Seed the random number generator                                                                     |
| 2       | permutation | Return a random permutation of a sequence, or return a permuted range                                |
| 3       | shuffle     | Randomly permute a sequence in-place                                                                 |
| 4       | rand        | Draw samples from a uniform distribution                                                             |
| 5       | randint     | Draw random integers from a given low-to-high range                                                  |
| 6       | randn       | Draw samples from a normal distribution with mean 0 and standard deviation 1 (MATLAB-like interface) |
| 7       | binomial    | Draw samples from a binomial distribution                                                            |
| 8       | normal      | Draw samples from a normal (Gaussian) distribution                                                   |
| 9       | beta        | Draw samples from a beta distribution                                                                |
| 10      | chisquare   | Draw samples from a chi-square distribution                                                          |
| 11      | gamma       | Draw samples from a gamma distribution                                                               |
| 12      | uniform     | Draw samples from a uniform [0, 1) distribution                                                      |

## Importing image data into NumPy array

| Sr. No. | Function     | Description                          |
| ------- | ------------ | ------------------------------------ |
| 1       | import PTL   | import pillow library                |
| 2       | import Image | import Image library                 |
| 3       | open         | open an image                        |
| 4       | format       | format of an image                   |
| 5       | size         | size of an image                     |
| 6       | mode         | mode of an image                     |
| 7       | type         | type of an image                     |
| 8       | imread       | load image as pixel array            |
| 9       | convert      | convert tje image `L` for grey scale |
| 10      | save         | save image                           |

## Advanced Array Manipulation Appendix

| Sr. No. | Function          | Description                                                             |
| ------- | ----------------- | ----------------------------------------------------------------------- |
| 1       | reshape           | reshape the array to desired shape                                      |
| 2       | ravel             | to lower dimension                                                      |
| 3       | flatten           | to lower dimension with a copy                                          |
| 4       | concatenate       | Most general function, concatenates collection of arrays along one axis |
| 5       | vstack, row_stack | Stack arrays row-wise (along axis 0)                                    |
| 6       | hstack            | Stack arrays column-wise (along axis 1)                                 |
| 7       | column_stack      | Like hstack, but converts 1D arrays to 2D column vectors first          |
| 8       | dstack            | Stack arrays “depth”-wise (along axis 2)                                |
| 9       | split             | Split array at passed locations along a particular axis                 |
| 10      | hsplit/vsplit     | Convenience functions for splitting on axis 0 and 1, respectively       |
| 11      | repeat            | replicates each element in an array some numberof times                 |
| 12      | tile              | a shortcut for stacking copies of an array along an axis                |
| 13      | take              | slice an array based on some other list                                 |
| 14      | put               | update array values                                                     |
