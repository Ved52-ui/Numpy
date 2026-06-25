# 🚀 NumPy Array Functions – Ultimate Cheat Sheet  

<p align="center">
  <img src="https://numpy.org/images/logo.svg" width="200" alt="NumPy Logo"/>
</p>
<p align="center">
  <b>A complete and beautiful guide to all major <code>NumPy</code> array functions.</b>  
  <br/> Learn NumPy faster with this handy cheat sheet! 
</p>
cvvvrvrv
---

## 📖 Table of Contents  
- [🌱 Array Creation](#-array-creation)  
- [🔎 Array Inspection](#-array-inspection)  
- [🔄 Reshaping & Transpose](#-reshaping--transpose)  
- [✂️ Indexing & Slicing](#️-indexing--slicing)  
- [🔗 Joining & Splitting](#-joining--splitting)  
- [➕ Mathematical Functions](#-mathematical-functions)  
- [📊 Statistical Functions](#-statistical-functions)  
- [🧮 Linear Algebra](#-linear-algebra-nplinalg)  
- [🔢 Set Operations](#-set-operations)  
- [🔍 Sorting & Searching](#-sorting--searching)  
- [📦 Broadcasting & Tiling](#-broadcasting--tiling)  
- [💾 Copying & Saving](#-copying--saving)  
- [📚 Resources](#-resources)  

---

## 🌱 Array Creation  

<details>
<summary>✨ Click to expand Array Creation functions</summary>

| Function | Description | Example |
|----------|-------------|---------|
| `np.array()` | Create array from list/tuple | `np.array([1,2,3])` |
| `np.zeros()` | Array of zeros | `np.zeros((2,3))` |
| `np.ones()` | Array of ones | `np.ones(4)` |
| `np.empty()` | Empty array (uninitialized) | `np.empty((2,2))` |
| `np.full()` | Filled with constant value | `np.full((2,2), 7)` |
| `np.arange()` | Range with step | `np.arange(1,10,2)` |
| `np.linspace()` | Evenly spaced numbers | `np.linspace(0,1,5)` |
| `np.logspace()` | Logarithmic spacing | `np.logspace(1,3,5)` |
| `np.eye()` | Identity matrix | `np.eye(3)` |
| `np.random.rand()` | Random values (0–1) | `np.random.rand(3,3)` |
| `np.random.randint()` | Random integers | `np.random.randint(1,10,(2,3))` |

</details>

---

## 🔎 Array Inspection  

<details>
<summary>👀 Click to expand Array Inspection functions</summary>

| Function | Description |
|----------|-------------|
| `arr.shape` | Dimensions of array |
| `arr.ndim` | Number of dimensions |
| `arr.size` | Total elements |
| `arr.dtype` | Data type |
| `arr.itemsize` | Size of one element (bytes) |
| `arr.nbytes` | Total memory used |

</details>

---

## 🔄 Reshaping & Transpose  

<details>
<summary>🔁 Click to expand Reshaping functions</summary>

| Function | Description |
|----------|-------------|
| `np.reshape(arr, (rows,cols))` | Reshape array |
| `arr.ravel()` | Flatten |
| `arr.flatten()` | Flatten (copy) |
| `arr.T` | Transpose |
| `np.swapaxes(arr,0,1)` | Swap axes |
| `np.expand_dims(arr,axis=0)` | Add axis |
| `np.squeeze(arr)` | Remove single-dim axis |

</details>

---

## ✂️ Indexing & Slicing  

<details>
<summary>✏️ Click to expand Indexing examples</summary>

```python
arr[1:5, 2:4]      # Slice
arr[arr > 5]        # Boolean indexing
arr[[1, 3, 5]]      # Fancy indexing
