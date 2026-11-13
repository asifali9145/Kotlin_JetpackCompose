# Kotlin_JetpackCompose 
**https://chatgpt.com/c/6af018cc-f9a8-83ee-896d-71f05ba21bcc**

**//==> Dated 12Nov26**

**Today's learning objectives:** 
1. Classes and Objects
2. Primary and Secondary Constructors
3. Inheritance
4. Data Classes
5. Companion Objects
6. Practical Android example

**1. Classes and Objects**
Sabse pehle samjhein:
**- Class:** Ek blueprint/template hoti hai.
**- Object:** Class ka actual instance hota hai.
**Example:** Agar aap Car class banate hain, to us class se Honda, Toyota ya Suzuki ke objects bana sakte hain.

**Java approach**
public class Car {
    String brand;
    int modelYear;
    void start() {
        System.out.println("Car Started");
    }
}
**Kotlin approach**
class Car {
    var brand: String = ""
    var modelYear: Int = 0
    fun start() {
        println("Car Started")
    }
}

**2. Constructors**
Constructor ka kaam object create hote waqt initial values provide karna hai.

Kotlin mein primarily do types hain:
- Primary Constructor
- Secondary Constructor

<img width="966" height="450" alt="image" src="https://github.com/user-attachments/assets/70839e5a-d67b-4633-8e6c-8e76c28e67f4" />
**4. Java vs Kotlin Comparison**
**Feature**	                          **Java**	                      **Kotlin**
Default constructor		       Compiler generated       	  No automatic constructor in same sense
No-argument constructor	            Yes		          	                    Yes
Parameterized constructor	          Yes		          	                    Yes
Multiple constructors	              Yes	                                  Yes
Constructor overloading	            Yes                                   Yes
Primary constructor	            No separate concept	                      Yes
Secondary constructor	          No separate concept	                      Yes

**Table ke Tamam Points ki Wazahat**
• **Default constructor.** Java mein agar aap koi constructor nahi banatay, to compiler khud ek khali constructor bana deta hai. 
                           Kotlin mein bhi agar aap koi constructor na likhein to compiler ek khali primary constructor banata hai, lekin agar aapne koi parameter wala constructor bana 
                           liya to khali constructor khud nahi banta (is liye table mein likha hai ke bilkul Java jaisa automatic system nahi hai).
• **No-argument constructor.**   Dono languages mein aap bina kisi parameter (argument) ke khali constructor bana saktay hain, jaise class Car().
• **Parameterized constructor**. Dono languages mein aap data pass karne ke liye parameters wale constructors bana saktay hain, jaise aapne apni pichli misal mein brand aur model pass kiya tha.
• **Multiple constructors.**     Dono languages mein ek hi class ke andar ek se zyada constructors banaye ja saktay hain.
• **Constructor overloading.**   Dono languages mein alag-alag parameters ke saath ek hi naam ke constructors (overloading) likhay ja saktay hain. Kotlin mein yeh kaam 
                                 Secondary constructors ya Default arguments se hota hai.
• **Primary constructor.**       Java mein primary constructor ka koi alag concept nahi hota, jabke Kotlin mein class header ke saath hi primary constructor likha jata hai.
• **Secondary constructor.**     Java mein saare constructors ek hi tarah se class ke andar likhay jatay hain (unhein secondary nahi kaha jata), jabke Kotlin mein primary constructor ke 
                                 ilawa jo bhi constructor body mein likha jaye usay Secondary constructor kehtay hain.

