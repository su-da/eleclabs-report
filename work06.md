# 三极管共射极放大电路

## 预习要求

1.  根据三极管型号查询有关资料，根据元器件参数估算电路关键点的电压、
    电流、电阻等数值。了解有哪些失真现象，各有何特点。

2.  了解电解电容正负极的使用要求。

3.  根据电路图做电路焊接。注意先通读实验讲义上的实验过程，了解哪部分
    电路需要留有余地。比如 RW~1~ 要换为固定电阻加电位器的串联；电容 C~1~
    和 C~2~ 的极性；R~L~ 要可通可断可更换；输入端可方便串入电阻。

4.  了解毫伏表的使用。

## 一些注意事项和说明

1.  图 [@fig:ex4notes]、[@fig:ex4notesDC]、[@fig:ex4noteswave] 分别是
    讲义上的电路图、其静态工作点及输出波形。输入信号的 Vpk 指幅度 (峰值、
    振幅)。注意图中所用的三极管与实验实际使用的略有不同，故这里的计算或
    仿真结果仅供参考。

![讲义上的电路](work06/bjt1.pdf) {#fig:ex4notes}

![静态工作点一](work06/bjt1DC.pdf) {#fig:ex4notesDC}

![输出波形一](work06/bjt1wave.pdf) {#fig:ex4noteswave}

2.  思考一下不采用负电源会怎么样？图 [@fig:ex4ce]、[@fig:ex4cedc]、
    [@fig:ex4cewave] 分别是该方案电路图、其静态工作点及输出波形。

![单电源共射极放大电路](work06/bjt2.pdf) {#fig:ex4ce}

![静态工作点二](work06/bjt2DC.pdf) {#fig:ex4cedc}

![输出波形二](work06/bjt2wave.pdf) {#fig:ex4cewave}

3.  一般资料上给出的共射极放大电路如图 [@fig:ex4ref] 所示。其静态工作
    点及输出波形分别如图 [@fig:ex4refdc] 和 [@fig:ex4refwave] 所示。
    与前面的电路进行比较。

![无基极串联电阻电路](work06/bjt3.pdf) {#fig:ex4ref}

![静态工作点三](work06/bjt3DC.pdf) {#fig:ex4refdc}

![输出波形三](work06/bjt3wave.pdf) {#fig:ex4refwave}

4.  图 [@fig:ex4ref] 中的 R5 改为 \SI{92.5}{\kilo\ohm}，其静态工作点如图
    [@fig:ex4refdc2] 所示。输入信号振幅为 \SI{5}{mV} 时的输出波形如图
    [@fig:ex4refwave2]。

![静态工作点四](work06/bjt4DC.pdf) {#fig:ex4refdc2}

![输出波形四](work06/bjt4wave.pdf) {#fig:ex4refwave2}

5.  图 [@fig:ex4ref] 中的 R5 改为 \SI{85}{k\ohm}，其静态工作点如图
    [@fig:ex4refdc3] 所示。输入信号振幅为 \SI{10}{mV} 时的输出波形如图
    [@fig:ex4refwave3]。

![静态工作点五](work06/bjt5DC.pdf) {#fig:ex4refdc3}

![输出波形五](work06/bjt5wave.pdf) {#fig:ex4refwave3}

6.  将图 [@fig:ex4ce] 中的 R2 改为与 C1 串联，如图 [@fig:ex4hi] 所示。调
    整基极偏置电阻，使得集电极电流 I~CQ~ 为 \SI{2}{mA}，其静态工作点如图
    [@fig:ex4hidc]，输出波形如图 [@fig:ex4hiwave]。注意比较以上 2、3、4、5
    所述各电路在静态工作点、放大倍数和可接受的输入电压的区别。

![输入端串联电阻的电路](work06/bjt6.pdf) {#fig:ex4hi}

![静态工作点六](work06/bjt6DC.pdf) {#fig:ex4hidc}

![输出波形六](work06/bjt6wave.pdf) {#fig:ex4hiwave}

对以上各电路做出思考和分析。注意实验时采用**图 [@fig:ex4ce]
($I_{\mathrm{CQ}}=\SI{1.5}{mA}$) 或图 [@fig:ex4hi]
($I_{\mathrm{CQ}}=\SI{2}{mA}$)**所示的电路。因实际采用的偏置电阻在
\SI{100}{k\ohm} 左右，所以应将 R5 改为**一个固定电阻
(\SIrange{10}{50}{k\ohm}) 与一个 \SI{100}{k\ohm} 电位器串联**。

实验时注意各仪器的共地，实验过程中所有述及的有关数据都要记录，数据记录
应清楚详尽，切忌混乱随意。如无说明，讲义上提及的信号电压为有效值。

讲义中要求用毫伏表测量交流信号的有效值，因实验室缺少毫伏表，此测量可以
用示波器代替。注意用示波器测量时分清峰峰值 (V~pp~)，峰值 (V~p~，即振幅)，
有效值。

本实验有可能需要测量较宽的频率范围，要保证示波器及探头满足带宽要求。示波
器探头的 X10 比 X1 档带宽要大不少，要注意查看有关资料和数据确认是否满足
测量需要。一般用 X10 测量比较好，但前提是使用前必须做好**校正**，否则测
量数据不可靠。

因信号发生器有约 \SI{50}{\ohm} 的输出阻抗，所以其电压读数不准确，实际输
出大小与接入的电路有关，故输入电压的测量应以测量仪器实测为准。
