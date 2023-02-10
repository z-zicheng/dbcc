# Project Description
It is easy to find open source to help us on CAN dbc files to c code convertions. But unfortunately, few of tools can be found to convert CANFD dbc files to c code. This is a tools to solve that problem.
This is a tool to convert CAN and CANFD dbc files to c files which can be used to reduce the coding work on CAN or CANFD signals processing. It is only modifed on the part of c code generation and deleted comparing with original project. And all other function(csv convertiion /xml conversion/...) are removed here. You can see more details from the original site:https://github.com/howerj/dbcc
&nbsp; 

# How to Run
1. Compile the program:   
    ``` sh 
    chas@my_workstation:~/dbcc$ mkdir build
    chas@my_workstation:~/dbcc$ cd build
    chas@my_workstation:~/dbcc$ cmake ..
    chas@my_workstation:~/dbcc$ make 
    ```
2. Convert dbc file to c code: 
    ``` sh
    chas@my_workstation:~/dbcc/build$ ./dbcc ../tests/float_signal.dbc
    ```
    then, you will get two c files for signals parsing.
3. How to use the generated files.
    ```
    TBD
    ```

# Notice
You'd better to use [CANdb++](https://www.vector.com/cn/zh/products/products-a-z/software/candb/#c104632) to save your dbc file as a new copy and using the copied file to generate c code to avoid issue from not matched dbc writting style.
