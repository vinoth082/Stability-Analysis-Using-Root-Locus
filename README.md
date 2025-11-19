# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:

<img width="426" height="707" alt="image" src="https://github.com/user-attachments/assets/1d4e9efb-7c1a-42b3-a879-177a1b7df3dc" />

<img width="406" height="727" alt="image" src="https://github.com/user-attachments/assets/018bdfab-2bcb-45db-87df-28233df6eacf" />

<img width="335" height="492" alt="image" src="https://github.com/user-attachments/assets/5b658e83-ab0f-4222-8649-d8e713819c68" />


## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 
```
num=[1];
den=[1 15 50 0];
sys=tf(num,den);
rlocus(sys);
[k,poles]=rlocfind(sys)
```

## Output:
<img width="852" height="772" alt="image" src="https://github.com/user-attachments/assets/4df6ebcb-eb52-429d-9d20-4df304a43fb3" />
<img width="946" height="295" alt="image" src="https://github.com/user-attachments/assets/6c2765e5-6c31-4c52-9034-0a75e75633b4" />



## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is 744.5551
