# 用途
测试c++中写文件的不同写法的速度

# 编译
加上选项-std=c++11

# 测试结果
1.	$ ./Test_write_speed 50                                                     
Testing begin....
option1, 50MB: 129ms
option2, 50MB: 129ms
option3, 50MB: 128ms
option4, 50MB: 98ms
2. $ ./Test_write_speed 100
Testing begin....
option1, 100MB: 249ms
option2, 100MB: 257ms
option3, 100MB: 257ms
option4, 100MB: 196ms
3. $ ./Test_write_speed 300                                                    
Testing begin....
option1, 300MB: 731ms
option2, 300MB: 763ms
option3, 300MB: 762ms
option4, 300MB: 583ms
4. $ ./Test_write_speed 500                                                    
Testing begin....
option1, 500MB: 1239ms
option2, 500MB: 1271ms
option3, 500MB: 1268ms
option4, 500MB: 968ms

# 结论
unistd.h中的write更快
