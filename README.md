  **Week1: C++(Till Pointers)

📂 File Format

Save programs as: filename.cpp


▶️ Compile & Run

Windows:

g++ file.cpp -o file.exe

file.exe

Linux/Mac:

g++ file.cpp -o file

./file



---

🔹 Step 1: Hello World

Definition: The first basic program in C++ that prints output.
Syntax:

#include <iostream>

using namespace std;

int main(){

    cout << "Hello World";
    
}

Output:


Hello World


---

🔹 Step 2: endl vs \n

Definition: Both are used for new lines.

endl → newline + flush buffer

\n → only newline
Example:


cout << "Hi" << endl << "Bye\n";


---

🔹 Step 3: Variables & Data Types

Definition: Variables store data. Each type decides the kind of data.
Syntax:

int a=10;    // integer

float b=3.14; // decimal

char c='A';   // character

bool d=true;  // boolean



---

🔹 Step 4: Operators

Definition: Used to perform operations on variables.
Types: Arithmetic (+, -, *, /, %), Relational (==, !=, <, >), Logical (&&, ||, !)
Example:

int a=10, b=3;

cout << a/b;   // 3

cout << a%b;   // 1




---

🔹 Step 5: // vs /

Definition:

// → comment (ignored by compiler)

/ → division operator



---

🔹 Step 6: Conditionals

Definition: Used for decision-making in programs.
Syntax & Example:

if(a>0) cout<<"Positive";
else cout<<"Negative";

switch(a){
  case 1: cout<<"One"; break;
  default: cout<<"Other";
}


---

🔹 Step 7: Loops

Definition: Used to repeat tasks.
Syntax & Example:

for(int i=0;i<5;i++) cout<<i; // 0 1 2 3 4

while(a>0){ cout<<a--; }         // while loop

do{ cout<<a; }while(a>0);        // do-while loop



---

🔹 Step 8: Nested Loops

Definition: A loop inside another loop.
Example:

for(int i=1;i<=2;i++)

  for(int j=1;j<=2;j++)
  
    cout<<i<<","<<j<<" ";
    

Output:

1,1 1,2 2,1 2,2


---

🔹 Step 9: Break & Continue

Definition:

break → exits the loop


continue → skips current iteration

Example:


for(int i=1;i<=5;i++){

  if(i==3) continue;
  
  if(i==5) break;
  
  cout<<i<<" "; // 1 2 4
}


---

🔹 Step 10: Functions

Definition: A block of code that performs a task.
Syntax:

returnType functionName(parameters){
   // body
}

Example:

int add(int a,int b){ return a+b; }

int main(){ cout<<add(3,4); } // 7


---

🔹 Step 11: Arrays

Definition: Collection of elements of same type stored in sequence.
Syntax:

datatype arrayName[size];

Example:

int arr[3]={10,20,30};

for(int i=0;i<3;i++) cout<<arr[i];


---

🔹 Step 12: Strings

Definition: A sequence of characters. In C++, handled by string class.
Syntax:

string str = "Hello";

Example:

string s="Harsha";

cout<<s.length();   // 6

cout<<s.substr(1,3); // ars


---

🔹 Step 13: String Functions

Definition: Useful methods to modify and check strings.
Examples:

getline(cin,s);             // input full line

s.append(" BM");            // add text

s.erase(0,1);               // remove char at pos

cout<<s.compare("Hello");   // 0 if equal


---

🔹 Step 14: Pointers

Definition: A variable that stores the memory address of another variable.
Syntax:

datatype* ptr;

Example:

int a=10;

int* p=&a;

cout<<*p;   // 10

int arr[3]={1,2,3};

cout<<*(arr+1); // 2




**this is just a minimal resource ..please learn more about these topics 
