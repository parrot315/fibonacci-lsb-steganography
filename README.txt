Explanation on how to use the tool:

- To compile the tool, use the following command:
        g++ main.cpp classes/*.cpp -o main.exe
- To embed a message in an image, use the following command:
        ./main.exe -e <input_img> <output_img> <payload>
- To extract a message from an image, use the following command:
        ./main.exe -d <input_img> <output_payload>

For example:
        ./main.exe -e sample_bmp.bmp output_bmp.bmp test.txt
        Or
        ./main.exe -d output_bmp.bmp output_bmp.txt


Note:
- The tool supports PNG, BMP, and GIF images.
- The tool supports text or executable files as payloads.
- The tool uses Fibonacci LSB steganography to embed the message in the image.
- The embedding size of GIF images is really small compared to PNG and BMP, hence test it with small files.