# Arithmetic-operation-using-8086
# 8086 Assembly Language Programs for Arithmetic Operations

## AIM

To write and execute Assembly Language Programs to perform arithmetic operations for the 8086 microprocessor.

---

## APPARATUS REQUIRED

* Personal Computer with MASM Software

---

## 1. ADDITION

#### Algorithm

1. Initialize memory location in HL register.
2. Store 1st data.
3. Increment HL to enter 2nd data.
4. Move 2nd number to accumulator.
5. Decrement HL.
6. Add value in memory with accumulator.
7. Store result.
8. Stop.


## FLOW CHART
<img width="707" height="1024" alt="image" src="https://github.com/user-attachments/assets/b5a7062d-e294-47cd-9683-a40de25e82de" />


#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV CL,00H
MOV AX,[SI]
MOV BX,[SI+02H]
ADD AX,BX
JNC L1
INC CL
L1:
MOV [SI+04H],AX
MOV [SI+06H],CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table
<img width="643" height="263" alt="image" src="https://github.com/user-attachments/assets/434604fd-8307-4800-9c0a-0d7fdf1ac9b7" />


#### Manual Calculations

<img width="770" height="530" alt="image" src="https://github.com/user-attachments/assets/979e75dd-8bcf-4f79-9caf-eb494aa52a0b" />


---

## OUTPUT IMAGE FROM MASM SOFTWARE
<img width="631" height="378" alt="Screenshot 2025-09-05 144151" src="https://github.com/user-attachments/assets/30c03e0d-ae93-414f-895e-e2d8f088f107" />
<img width="647" height="406" alt="Screenshot 2025-09-05 144013" src="https://github.com/user-attachments/assets/01bbb3c2-652c-4b38-a4f4-9d2a30224f6b" />


## 2. SUBTRACTION

#### Algorithm

1. Initialize memory and store 1st data.
2. Increment to get 2nd data.
3. Move 2nd data to accumulator.
4. Subtract memory content.
5. Store result.

## FLOWCHART

<img width="578" height="797" alt="image" src="https://github.com/user-attachments/assets/564c3c7a-33ce-4a1c-8920-beb5c24b9b47" />


#### Program



#### Output Table

<img width="639" height="241" alt="image" src="https://github.com/user-attachments/assets/6cf69027-0a26-44fe-92bb-df687c6b640e" />


#### Manual Calculations

<img width="777" height="778" alt="image" src="https://github.com/user-attachments/assets/9db42ddc-67df-4d1a-a5d4-03c3078c4ce7" />


---


## OUTPUT SCREEN FROM MASM SOFTWARE
<img width="639" height="399" alt="Screenshot 2025-09-05 144531" src="https://github.com/user-attachments/assets/7f41f76c-6c37-4bb3-93d5-f2d12624924e" />
<img width="624" height="427" alt="Screenshot 2025-09-05 144736" src="https://github.com/user-attachments/assets/01b4e9e2-3fc2-4860-a0c3-d3efdf9d8289" />


## 3. MULTIPLICATION

#### Algorithm

1. Initialize memory and store operands.
2. Move operands to registers.
3. Multiply.
4. Store result.

##FLOWCHART

<img width="569" height="906" alt="image" src="https://github.com/user-attachments/assets/88be88ff-2896-4a88-b73d-84ccffd2fcf9" />



#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
MUL BX
MOV [SI+04H],AX
MOV [SI+06H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

<img width="644" height="246" alt="image" src="https://github.com/user-attachments/assets/ad8ef3bd-141a-4792-b02b-8a163d74747c" />


#### Manual Calculations

<img width="777" height="747" alt="image" src="https://github.com/user-attachments/assets/97c86c63-8c0d-43d9-bb74-0ef6641e336b" />

---

## OUTPUT SCREEN FROM MASM SOFTWARE
<img width="639" height="429" alt="Screenshot 2025-09-05 151703" src="https://github.com/user-attachments/assets/f18339d5-011d-4a2f-ac51-e5388524d842" />
<img width="624" height="417" alt="Screenshot 2025-09-05 145605" src="https://github.com/user-attachments/assets/d3f27c04-f509-4ca6-88b8-d4c57f5def69" />


## 4. DIVISION

#### Algorithm

1. Load memory location of operands.
2. Perform division.
3. Store result.

   ## FLOWCHART
<img width="1065" height="802" alt="image" src="https://github.com/user-attachments/assets/25b4a483-0d42-494b-8639-1af3ea17191b" />


#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
DIV BX
MOV [SI+04H],AX
MOV [SI+06H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table
<img width="646" height="244" alt="image" src="https://github.com/user-attachments/assets/d74bca29-f0bc-4569-850a-c51b51c11483" />

#### Manual Calculations
<img width="750" height="668" alt="image" src="https://github.com/user-attachments/assets/384f5f14-858f-4cad-b374-e1b8f4b3005c" />
---


## OUTPUT FROM MASM SOFTWARE
<img width="636" height="429" alt="Screenshot 2025-09-05 151805" src="https://github.com/user-attachments/assets/5ba80895-5ea6-412d-8d55-4c9a651322ca" />
<img width="638" height="432" alt="Screenshot 2025-09-05 151535" src="https://github.com/user-attachments/assets/5f76ff9e-f2f4-4506-96d0-8bc0ec880c73" />

## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.

---
