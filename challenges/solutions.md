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
32-i: echo "Hello"; sleep 5; echo "World!"
33-i: dd if=/dev/zero of=32zero.bin bs=1000 count=1
34-i: dd if=/dev/urandom of=34random.bin bs=2000 count=1
35-i: wc -l /home/gabrielcortez/Documents/command-line-challenges/README.txt 
36-b: tac /home/gabrielcortez/Documents/command-line-challenges/README.txt
37-i:  cut -d ',' -f 2 people.csv 
38-a: cut -d ',' -f 2 people.csv |sort| uniq | wc -l
39-a: cut -d ',' -f 2 people.csv | tail -n +2 | sort | uniq | wc -l
40-a: awk 'NR > 1 {print $2}' people.csv | sort | uniq | wc -l
41-a: 
time cut -d ',' -f 2 people.csv | tail -n +2 | sort | uniq | wc -l
time awk 'NR > 1 {print $2}' people.csv | sort | uniq | wc -l
42-a: tail -n +2 people.csv | cut -d ',' -f 4 | grep -c "^Josiah$"
43-i: find -type f | wc -l
44-i: find -mindepth 1 -type d | wc -l
45-i: find . -type f -name "*deleteme*" -delete
46-i: sed -i 's/You found the needle in the haystack!/The needle has been removed./g' $(grep -rl "You found the needle in the haystack!" bunch_of_files/)
47-i: sed 's/,/|/g' people.csv > people_pipe.csv
48-a: find bunch_of_files -type f -exec md5sum {} + | grep $(md5sum bunch_of_files/file001.rand | awk '{print $1}')
49-a: 
touch touch supercalifragilisticexpialidocious.txt
rm !$
50-a: touch {a..c}-{1..3}.txt










