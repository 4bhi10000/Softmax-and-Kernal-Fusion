Softmax and Kernel Fusion experiment
1. Extract all files into D:\Softmax_experiment
2. Open Command Prompt in that folder
3. Compile: nvcc -arch=sm_75 softmax_fusion.cu -o softmax_fusion.exe
4. Run: softmax_fusion.exe
5. Install graph packages if needed: py -m pip install pandas matplotlib
6. Generate graphs: py create_graph.py

RTX 2050 uses compute capability 8.6, so use -arch=sm_86 if supported by your installed CUDA toolkit.
The program reports measured timings; do not assume fusion is always faster.
