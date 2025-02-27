# Huffman Coding Compression and Decompression Tool

# Overview

This tool provides a simple implementation of Huffman coding for text file compression and decompression. It uses a binary tree to encode and decode text files.

# Features

- Compresses text files using Huffman coding
- Decompresses compressed files back to their original text format
- Handles padding and removal of padding during compression and decompression

# Usage

1. Run the script and enter the path of the text file you want to compress.
2. The script will compress the file and save it as a binary file (.bin).
3. The script will then decompress the binary file and save the original text in a new file (_decompressed.txt).

# Code Structure

The code consists of two main classes:

- BinaryTree: Represents a binary tree node with a value, frequency, and left and right child nodes.
- HuffmanCode: Handles the compression and decompression process using Huffman coding.

# Methods

- frequency_from_text(text): Calculates the frequency of each character in the given text.
- build_heap(frequency_dic): Builds a min-heap from the frequency dictionary.
- __Build_binary_tree(): Constructs the Huffman binary tree from the min-heap.
- __Build_tree_code(): Builds the Huffman code dictionary from the binary tree.
- __Build_encoded_text(text): Encodes the given text using the Huffman code dictionary.
- __build_padded_text(encoded_text): Pads the encoded text to make its length a multiple of 8.
- __build_bits_array(padded_text): Converts the padded text into a byte array.
- compression(): Compresses the input file using Huffman coding.
- decompress(input_path): Decompresses the compressed file back to its original text format.

# Example Use Case

Enter the path of your file which you need to compress: /path/to/your/file.txt

The script will compress the file and save it as /path/to/your/file.bin.

Then, it will decompress the binary file and save the original text in a new file /path/to/your/file_decompressed.txt.
