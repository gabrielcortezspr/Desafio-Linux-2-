p1-b: tar -xzf challenges.tar.gz 
p2-b: cd challenges/
p3-b: ls -1
p4-b: mkdir foo
p5-b: mdfir -p foo/bar/1/2/3
p6-b: rm -r foo
p7-b: echo "Hello World"
p8-b: echo "Hello World" > hello.txt
p9-b: touch empty.txt
p10-b: rm empty.txt
p11-i: printf "Hello World" > hello.txt
p12-i: "Hello World"|tee hello
p13-b: cp hello.txt goodbye.txt
14-b: mv goodbye.txt hello.txt
p15-i: diff hello.txt hello_copy.txt
p16-b: cat hello.txt hello_copy.txt > 2_hellos.txt
p17-b: pwd
p18-b: ls -l
p19-b: echo "Testando" >> restricted.txt
p20-b: ./hello_executable
p21-b: 
chmod +x challenge_20 
./challenge_20
p22-b:
gcc compile_me.c -o compile_me
./compile_me
p23-a: ./redirect > output.txt
p24-b: date
p25-b: ps aux
p26-b: nproc
27-b: uname -r
28-b: grep -r "You found the needle in the haystack!" bunch_of_files/
29-b: head -25 people.csv
30-b: tail -25 people.csv
31-i: diff greeting1.txt greeting2.txt



















