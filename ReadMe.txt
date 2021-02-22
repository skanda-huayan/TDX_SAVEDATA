#TDX Save Data for day's K line#

1 編譯
VS2015

2 綁定公式
1）把DLL文件放在，到通達信安裝目錄的T0002/dlls之下
2）綁定DLL函數。假設綁在3號DLL。
3）添加公式：
SHL:=TDXDLL3(1,Code,H,L);
SOC:=TDXDLL3(2,Code,O,C);
SDA:=TDXDLL3(3,Code,Date,0);
TDXDLL3(4,0,0,0);
