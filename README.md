Author: Isaac Browen <br>
LLM Model: **Chat-GPT 4o mini** <br>
Question: How has the syntax and keywords in programming languages evolved over time? How have newer programming languages changed their syntax?

## References <span style="font-size:16">(in order of apperance)</span>
- [Bjarne Stroustrup, _The C++ Programming Language_](https://cds.cern.ch/record/169940/files/cer-000081326.pdf); [Guido van Rossum, _Python Language Reference_](https://scicomp.ethz.ch/public/manual/Python/3.10.4/reference.pdf)
- [Backus et al., 1957](https://dl.acm.org/doi/pdf/10.1145/960118.808380)
- [Van Rossum, G., *Python Tutorial*](https://dev.rbcafe.com/python/python-3.5.1-pdf/tutorial.pdf)
- [Bloch, J., *Effective Java*](https://books.google.com/books?hl=en&lr=&id=BIpDDwAAQBAJ&oi=fnd&pg=PT10&dq=Joshua+Bloch,+Effective+Java+-&ots=LyaKfbMY36&sig=ihahwrK6Lucx-eVrjv0QBbKTHcE#v=onepage&q=Joshua%20Bloch%2C%20Effective%20Java%20-&f=false)
- [Hennessy & Patterson, _Computer Architecture: A Quantitative Approach_](https://books.google.com/books?hl=en&lr=&id=cM8mDwAAQBAJ&oi=fnd&pg=PP1&dq=Hennessy+%26+Patterson,+_Computer+Architecture:+A+Quantitative+Approach_&ots=SJXaFkZVsd&sig=7YR5hi0w6jSeWsVevWut3E5nm9s#v=onepage&q=Hennessy%20%26%20Patterson%2C%20_Computer%20Architecture%3A%20A%20Quantitative%20Approach_&f=false)
- [Patterson & Hennessy, _Computer Organization and Design: The Hardware/Software Interface_](https://books.google.com/books?hl=en&lr=&id=Pz-XCgAAQBAJ&oi=fnd&pg=PP1&dq=Patterson+%26+Hennessy,+_Computer+Organization+and+Design:+The+Hardware/Software+Interface_&ots=GcMb_msXeX&sig=cZIj-Isl7rwzE2DtEoi5PWfVJak#v=onepage&q=Patterson%20%26%20Hennessy%2C%20_Computer%20Organization%20and%20Design%3A%20The%20Hardware%2FSoftware%20Interface_&f=false)
- [Silberschatz, Korth, & Sudarshan, _Database System Concepts_](https://people.inf.elte.hu/kiss/DB/dbms_korth_soln.pdf)
- [Tanenbaum, _Modern Operating Systems_](https://www.nastooh.com/teaching/Modern_Operating_System_Tanenbaum_3rd_edition.pdf)
- [Stallings, _Operating Systems: Internals and Design Principles_](https://dl.acm.org/doi/abs/10.5555/2012029)

## Concepts
- Early and Modern Programming Languages
- Technological Advances
- Operating System Features
- Virtual Memory
- Paging & Segmentation

## Part 1 :: Answer the Question
>**_To limit the amount of long answers and AI hallucinations additional commands were given to the AI before asking the question here is the command that it was given:_** For this conversation I will be asking you a question about programming languages. You will respond in an attempt to answer this question using academic resources and references when possible. In general keep responses limited to at most five sentences. Do not make things up! Do not repeat yourself!

**How has the syntax and keywords in programming languages evolved over time? How have newer programming languages changed their syntax?**
### GPT
The evolution of syntax and keywords in programming languages reflects a shift towards greater readability, expressiveness, and abstraction. Early languages like Fortran and Assembly used minimalistic syntax focused on machine efficiency, while languages like C introduced more structured control flow and data types.

In the 1990s, object-oriented languages like C++ and Java introduced new keywords and syntax to support encapsulation, inheritance, and polymorphism, aiming to enhance code reusability and maintainability. More recently, languages such as Python and JavaScript have embraced dynamic typing and flexible syntax to streamline development and reduce verbosity, emphasizing ease of use and rapid prototyping. This evolution highlights a trend toward syntax that prioritizes developer productivity and code clarity over low-level machine optimization ([Bjarne Stroustrup, _The C++ Programming Language_](https://cds.cern.ch/record/169940/files/cer-000081326.pdf); [Guido van Rossum, _Python Language Reference_](https://scicomp.ethz.ch/public/manual/Python/3.10.4/reference.pdf)).

### GPT : Examples of the same program in different languages

##### **Fortran (1950s):**
```Fortran
PROGRAM HelloWorld
PRINT *, 'Hello, World!'
END PROGRAM HelloWorld
```

##### **C (1970s):**

```C
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

##### **Java (1990s):**
```Java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

##### **Python (1990s):**
```Python
print(“Hello World”)
```

##### **JavaScript (1990s):**
```JavaScript
console.log(“Hello World”);
```

**Above answer provided by GPT**, Question: “can you provide written examples showing the differences between the code of each language?”

### ME
How were the early languages like Fortran focused on machine efficiency what does that mean and why would modern languages be considered less efficient?
### GPT
Early languages like Fortran were designed with a strong emphasis on machine efficiency. They were optimized for the hardware capabilities of their time, such as memory and processing speed. Fortran, for example, allowed programmers to write code that was very close to the machine’s native instructions, which minimized the overhead and maximized performance for numerical and scientific computations ([Backus et al., 1957](https://dl.acm.org/doi/pdf/10.1145/960118.808380)).

This efficiency was achieved by providing low-level access to system resources, simple syntax, and direct control over memory and processor usage. Fortran’s design focused on minimizing abstraction layers between the code and the machine’s hardware, which could result in faster execution times and better use of system resources.

Modern languages, such as Python or Java, often trade some of this low-level efficiency for higher-level abstractions that improve developer productivity, code readability, and maintainability. For instance, Python handles memory management automatically via garbage collection and provides high-level constructs that simplify complex tasks but can introduce performance overhead compared to lower-level languages. These languages are designed to be more user-friendly and versatile, often at the cost of raw performance ([Van Rossum, G., *Python Tutorial*](https://dev.rbcafe.com/python/python-3.5.1-pdf/tutorial.pdf); [Bloch, J., *Effective Java*](https://books.google.com/books?hl=en&lr=&id=BIpDDwAAQBAJ&oi=fnd&pg=PT10&dq=Joshua+Bloch,+Effective+Java+-&ots=LyaKfbMY36&sig=ihahwrK6Lucx-eVrjv0QBbKTHcE#v=onepage&q=Joshua%20Bloch%2C%20Effective%20Java%20-&f=false)).

## Part 2 :: Question Confusion 
>At this point in my exploration of the topic I realized that the AI was interpreting this question in a way I hadn’t intented. The question I had in my head was one about how specific keywords have changed overtime, like how Assembly has mov, add, xor while Python has operators like + and function like print(). I wanted to learn about why these keywords changed as programming languages evolved. However, the answers I was getting from GPT were more about how and why entire new langauges were created and how they automated tasks for the programmers. This is something that I haden’t conciered when first drafting my question I had assumed that new programming languages were simply changing how code was displayed by using different keywords for different tasks. But the AI reminded me that modern languages are also automating a large number of tasks that older langauges made the programmer do. One of the first things we learn in CPSC 231 is that Java has an automatic garbage collector. In that class we don’t know enough about code or computers to know what that means and it isn’t until we get to C++ that we learn that the computer has to be told what to do with every value. It won’t just forget a variable unless we tell it to, and in Java the langauge and compiler was doing that for us. So when I asked the AI to explain how programming langauges had changed over time that is the answer it gave me, modern programming languages have abstracted tasks away from the user to allow for a higher level, more human readable, programming expereince.

>With this in mind I began to ask the AI more about what inovations allowed things like garbage collection to become automated.

### ME
what specific change in technology allowed program designers to shift away from low level memory management to higher level abstracted languages?
### GPT 
The shift from low-level memory management to higher-level abstraction languages was primarily enabled by advancements in **hardware capabilities** and **operating system technologies**.

1. **Increased Processing Power**: As computer processing power improved, it became feasible for hardware and operating systems to handle more complex tasks ([Hennessy & Patterson, _Computer Architecture: A Quantitative Approach_](https://books.google.com/books?hl=en&lr=&id=cM8mDwAAQBAJ&oi=fnd&pg=PP1&dq=Hennessy+%26+Patterson,+_Computer+Architecture:+A+Quantitative+Approach_&ots=SJXaFkZVsd&sig=7YR5hi0w6jSeWsVevWut3E5nm9s#v=onepage&q=Hennessy%20%26%20Patterson%2C%20_Computer%20Architecture%3A%20A%20Quantitative%20Approach_&f=false)).
	- **Enhanced Hardware Capabilities**: As CPU performance improved, computers became capable of executing more complex and resource-intensive tasks efficiently. This increase in processing power made it feasible to implement sophisticated memory management features, such as garbage collection, without significantly impacting performance.
	- **Larger Memory and Storage**: The expansion in available RAM and storage meant that programs could rely on the operating system and hardware to handle memory allocation and deallocation more efficiently. With more memory available, it became practical to use automated systems as there was less concern about running out of resources.
	- **Improved Hardware Abstractions**: Advances in processor architecture introduced features like memory management units (MMUs) and virtual memory, which abstracted physical memory management away from the programmer. This allowed higher-level languages to incorporate memory management features that would have been impractical with earlier hardware ([Patterson & Hennessy, _Computer Organization and Design: The Hardware/Software Interface_](https://books.google.com/books?hl=en&lr=&id=Pz-XCgAAQBAJ&oi=fnd&pg=PP1&dq=Patterson+%26+Hennessy,+_Computer+Organization+and+Design:+The+Hardware/Software+Interface_&ots=GcMb_msXeX&sig=cZIj-Isl7rwzE2DtEoi5PWfVJak#v=onepage&q=Patterson%20%26%20Hennessy%2C%20_Computer%20Organization%20and%20Design%3A%20The%20Hardware%2FSoftware%20Interface_&f=false)).

2. **Advanced Operating Systems**: Modern operating systems introduced features like virtual memory and advanced memory management techniques. These systems abstracted low-level hardware interactions from the programmer, allowing higher-level languages to provide simpler, more intuitive interfaces for managing resources ([Silberschatz, Korth, & Sudarshan, _Database System Concepts_](https://people.inf.elte.hu/kiss/DB/dbms_korth_soln.pdf)).
	- **Virtual Memory**: Modern operating systems use virtual memory to provide the illusion of a large, contiguous memory space to applications, even if physical memory is fragmented or limited. This allows programs to run without needing to manage physical memory directly. Virtual memory also supports features like paging and swapping, where parts of programs and data can be moved between RAM and disk storage as needed.
	- **Memory Protection and Isolation**: Advanced operating systems implement memory protection mechanisms that prevent one program from accessing or modifying the memory space of another. This isolation enhances system stability and security, allowing higher-level languages to assume that their memory allocations are safe from interference by other processes ([Tanenbaum, _Modern Operating Systems_](https://www.nastooh.com/teaching/Modern_Operating_System_Tanenbaum_3rd_edition.pdf)).
	- **Garbage Collection**: Many modern operating systems and runtime environments incorporate garbage collection, which automatically handles the allocation and deallocation of memory. This eliminates the need for programmers to manually manage memory, reducing the risk of memory leaks and dangling pointers. Garbage collectors can reclaim memory used by objects that are no longer referenced by the program, improving overall memory efficiency and reducing programming complexity.
	- **Advanced Scheduling and Resource Management**: Operating systems have developed sophisticated scheduling algorithms and resource management techniques to efficiently allocate CPU time and other resources to different processes. These advancements allow high-level languages to rely on the OS for efficient multitasking and resource utilization, rather than requiring explicit management by the programmer ([Stallings, _Operating Systems: Internals and Design Principles_](https://dl.acm.org/doi/abs/10.5555/2012029)).

## Part 3 :: Operating System Interest 
>The mention of improvements in operating system interested me. In my classes I’ve learned about how program compilers and system memory have imporved to allow for more advanced operations but I’ve heard nothing about how imporvements in operating system have contributed to improvements in programming languages. This interested prompted the next line of questioning.
### ME
explore the theory behind virtual memory
### GPT
Virtual memory allows a computer to use more memory than it physically has by creating an abstract, large memory space for each process. It achieves this by using hardware and software to manage memory in a flexible way. The operating system uses techniques like **paging and segmentation** to break memory into manageable pieces. When a program accesses a memory location, the system translates this address and loads the required data from disk into RAM if it's not already there. This approach not only extends available memory but also improves multitasking and process isolation by preventing one process from interfering with another.
### ME
elaborate further on paging and segmentation
### GPT
**Paging:** Paging divides memory into fixed-size blocks called "pages." Each page is a small, contiguous block of memory that can be independently mapped between virtual and physical memory. When a program accesses memory, the virtual address is divided into a page number and an offset. The operating system uses a page table to translate the virtual page number into a physical page frame in RAM. If the required page is not in RAM, it's loaded from disk storage, a process known as "paging in." This method simplifies memory management and makes it easier to handle processes that need more memory than is physically available.

**Segmentation:** Segmentation divides memory into variable-sized blocks called "segments," each representing a logical unit of data or code, such as a function or an array. Unlike paging, which uses fixed-size blocks, segmentation allows for more flexible and meaningful organization of memory. Each segment has a starting address and a length, and the system keeps a segment table to map these segments from virtual to physical memory. This approach helps manage memory based on the structure of the program rather than fixed-size pages, allowing for more efficient use of memory for different types of data and code.

##### Vendiagram : Paging & Segmentation
**Paging:**
- Uses fixed-size pages
- Simple memory management
- Address divided into page number and offset

**Segmentation:**
- Uses variable-sized segments
- Memory organized by logical units
- Address divided into segment number and offset

**Shared Features:**
- Both use virtual memory
- Both involve address translation
- Can be combined in some systems (e.g., segmented paging)

_Paging and Segmentation Reference_ ([Patterson & Hennessy, _Computer Organization and Design: The Hardware/Software Interface_](https://books.google.com/books?hl=en&lr=&id=Pz-XCgAAQBAJ&oi=fnd&pg=PP1&dq=Patterson+%26+Hennessy,+_Computer+Organization+and+Design:+The+Hardware/Software+Interface_&ots=GcMb_msXeX&sig=cZIj-Isl7rwzE2DtEoi5PWfVJak#v=onepage&q=Patterson%20%26%20Hennessy%2C%20_Computer%20Organization%20and%20Design%3A%20The%20Hardware%2FSoftware%20Interface_&f=false))

## Conclusion
The evolution from low-level memory management to higher-level abstractions in programming languages reflects advancements in both hardware and software. Increased processing power has made it feasible for modern operating systems to handle complex memory management tasks like garbage collection, shifting the burden away from programmers. Virtual memory, utilizing techniques such as paging, allows for more efficient and flexible use of memory. These advancements have led to the development of high-level languages like Python, which prioritize readability and developer productivity over manual memory management. This transition demonstrates a balance between optimizing performance and enhancing readability of programming.
