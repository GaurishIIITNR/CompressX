# CompressX

CompressX is a web-based file compression and decompression tool developed using HTML, CSS, and JavaScript. It employs Huffman's Algorithm and Heap data structures to achieve efficient and lossless compression of files. This README provides an overview of the project.

## Table of Contents

- [Features](#features)
- [Workflow](#Workflow)

## Features

- Compress files to reduce their size while maintaining data integrity.
- Decompress files to their original state.
- Utilizes Huffman's Algorithm to achieve high compression efficiency.
- User-friendly web interface for easy file selection and interaction.
- Supports a wide range of file formats for versatility.
- Cross-browser compatibility for a seamless user experience.

## Workflow

1. **File Selection**: Users begin by launching the CompressX web application and selecting the file they want to compress or decompress.

2. **Compression Process**:
   - When the user clicks the "Compress" button, the selected file undergoes the following process:
   - **Huffman Coding**:
     - The file is scanned to generate frequency statistics for each character or symbol.
     - A Huffman tree is constructed based on these frequencies, with shorter codes assigned to more frequent characters.
     - The Huffman tree is used to create a codebook, which maps characters to their respective Huffman codes.
     - The original file is then encoded using the generated Huffman codes.
   - **Heap Data Structure**:
     - A binary heap data structure is utilized to efficiently prioritize and store character frequencies during Huffman tree construction.
   - **Output Generation**:
     - The compressed data, along with the Huffman tree structure and any metadata, is saved as a compressed file.
     - This compressed file is made available for download to the user.

3. **Decompression Process**:
   - When the user clicks the "Decompress" button and selects a compressed file, the following steps occur:
   - The compressed file is read, and the Huffman tree structure and metadata are extracted.
   - Using the Huffman tree, the encoded data is decoded, resulting in the original file.
   - The original file is made available for download to the user.
   - 
## Key Components

### Huffman's Algorithm
- **Node**: Each node in the Huffman tree represents a character and its frequency.
- **Huffman Tree**: The tree is constructed by repeatedly merging nodes with the lowest frequencies until a single root node is formed.
- **Codebook**: A mapping of characters to their Huffman codes is created from the constructed tree.

### Heap Data Structure
- A binary heap is used to efficiently manage and prioritize character frequencies during Huffman tree construction.

### User Interface
- HTML, CSS, and JavaScript are employed to create an intuitive and user-friendly interface for file selection, compression, and decompression.

## Lossless Compression
- The use of Huffman's Algorithm ensures that data compression is lossless, meaning the original data can be perfectly reconstructed from the compressed data.

## Conclusion

CompressX combines efficient data compression techniques with a user-friendly web interface, making it a versatile tool for reducing file sizes while preserving data integrity.


