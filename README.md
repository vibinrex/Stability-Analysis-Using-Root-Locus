# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:

![WhatsApp Image 2025-11-15 at 08 33 34_f8acd44b](https://github.com/user-attachments/assets/e7751fa2-68f7-4040-8a15-3b0278472c06)

![WhatsApp Image 2025-11-15 at 08 34 00_a41a6a4b](https://github.com/user-attachments/assets/65a47494-32ea-40d2-89f5-6fcd45b654b6)

![WhatsApp Image 2025-11-15 at 08 34 25_4bbbe96f](https://github.com/user-attachments/assets/a41e8932-f9b8-4f72-874a-08ba3e718a0e)

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

<img width="1736" height="868" alt="Screenshot 2025-11-15 225939" src="https://github.com/user-attachments/assets/7a4012a2-03de-4cda-acd5-991c6cd577f8" />

<img width="274" height="275" alt="Screenshot 2025-11-15 074942" src="https://github.com/user-attachments/assets/ec62a2cb-5851-4706-898b-a4bd95e7f603" />

## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is 755
