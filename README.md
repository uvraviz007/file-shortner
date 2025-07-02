
# Huffman File Compressor

This is a simple C++ project that implements **Huffman Encoding and Decoding** for file compression and decompression. It reads a plain text file, compresses it using the Huffman coding algorithm, and generates a `.huf` file. It can also decode the `.huf` file back to its original form.

---

##  Features

-  Compresses any plain text file using Huffman coding.
-  Supports decompression from `.huf` back to original.
-  Binary file handling with custom metadata storage.
-  CLI interface: encode and decode via command line.
-  Written in standard C++ (cross-platform compatible).

---

##  File Structure

```
.
├── encode.cpp         # Main program to compress (encode)
├── decode.cpp         # Main program to decompress (decode)
├── huffman.cpp        # Class implementation
├── huffman.hpp        # Class declaration and data structures
├── index.html         # Huffman tree visualizer (Bootstrap + JS)
├── example.txt        # Sample input file
├── compressed.huf     # Compressed output
├── output.txt         # Final decompressed output
```

---

##  How to Compile

###  Encode (Compress)
---bash
g++ encode.cpp huffman.cpp -o encode


###  Decode (Decompress)
---bash
g++ decode.cpp huffman.cpp -o decode


---

##  How to Use

###  Compress a file
---bash
./encode example.txt compressed.huf


###  Decompress a file
---bash
./decode compressed.huf output.txt

##  Huffman Tree Visualizer (Bonus)

A browser-based Huffman Tree visualizer built with **HTML, Bootstrap 5, and JavaScript**.

###  How to use:
1. Open `index.html` in your browser:
   ---bash
   start index.html
   
2. Enter sample text and click **Generate Tree**.
3. Visual Huffman Tree will be rendered on screen.


##  Example

1. Prepare `example.txt` with some text.
2. Run:
   ```bash
   ./encode example.txt compressed.huf
   ./decode compressed.huf output.txt
   ```
3. Check:
   ```bash
   fc example.txt output.txt   # On Windows
   diff example.txt output.txt # On Linux/macOS
   ```

If no differences, your compression-decompression is working perfectly.

---

##  Concepts Used

- **Huffman Tree**
- **Priority Queue (Min-Heap)**
- **Binary Encoding**
- **Bit Manipulation**
- **File I/O (Binary and Text Modes)**

---



> Created by Ravi Sharma  
> B.Tech CSE, MNNIT  
> GitHub: [@uvraviz007](https://github.com/uvraviz007)

---



This project is for educational and personal use. Free to use and modify.
