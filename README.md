# Cpeater
Running the Linux command tools repeatedly.

*** You need to run this file in the directory, ~/Handmade_tools/Cpeater ***

## Installation
1. Download 'cpeater', 'help.txt' on the directory, ~/Handmade_tools/Cpeater.
2. echo 'export PATH=$PATH:$HOME/Handmade_tools/Cpeater' >> ~/.bashrc
source ~/.bashrc

## Usage
help.txt 읽으세영

### example
```
cpeater tblastn -subject SRR622542{}_selected.fasta 0-3 -query viral.1.protein.faa -outfmt '"6 std qlen"' -num_threads 30 -evalue 1e-10 -max_targe
t_seqs 1 -out result{}.fasta 10,20-22 
```
아 영어 쓰기 귗낳다 걍 저렇게 맨 앞에 박으시면 됩니다.

(Just stick it at the beginning like that.)

### Setting range
- {}에 들어갈 수들 입력하는 거는 개별로 입력하실 때는 , 쓰시구요 범위로 입력하실 때는 -하심 되구요 섞어서 쓸 수도 있어요.

(When entering values for {}, use a comma(,) for individual values and a hyphen(-) for ranges.)

- {} 안 쓰면 그냥 default로 그 값을 계속 쓰게 됩니다.

(If you omit {}, it will continue to use the default value.)

- 근데 범위 안 맞게 입력하면 안 굴러가요 당연한 기능.

(If you input the range incorrectly, it won't work. Basic functionality, obviously.)

### Enter the parameter
- 걍 평소 쓰듯이 쓰시면 되는데, 예제처럼 범위 지정할 부분에 {} 넣으시고 뒤에 범위 설정 하세요.

(Just write it as you normally would. For specifying ranges as shown in the example, put {} and set the range at the end.)

- parameter 순서는 신경쓰지 않습니다. 진짜 걍 쓰던대로 넣으시면 됨.

(The order of parameters doesn't matter. Just input them as you normally would.)

- 예제처럼 "" 넣을 때가 있는데, 그때는 ''로 감싸주시면 됩니다.

(In some cases, as in the example, when putting "<parameter>", if needed, enclose them in ''.('"<parameter>"'))
