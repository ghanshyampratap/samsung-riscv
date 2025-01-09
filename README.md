## Welcome to My Repository for the RISC-V Talent Development Program! 💡

Powered by Samsung Semiconductor India Research (SSIR) and VLSI System Design (VSD), this program is all about exploring the cutting-edge RISC-V architecture 🖥️. With the power of open-source tools 🛠️, we're offering hands-on experience in VLSI chip design 🧠 and the RISC-V architecture 🔧.

Get ready to dive into the world of innovative technology 🌐 and shape the future of chip design with us! Together, let's push the boundaries and unlock the full potential of RISC-V 💥.

## 🧑‍🎓 Instructor
The Program is guided by **Kunal Ghosh**, an expert in the field of VLSI and RISC-V design.

## 📋 Basic Information

- **Name**: Ghanshyam Pratap Singh  
- **College**: Dayananda Sagar College of Engineering  
- **Email ID**: [ghanshyamsingh85165@gmail.com](mailto:ghanshyamsingh85165@gmail.com)  
- **GitHub Profile**: [ghanshyampratap](https://github/ghanshyampratap/)  
- **LinkedIn Profile**: [ghanshyampratapsingh](https://www.linkedin.com/in/ghanshyampratapsingh/)  

---

# 🚀 Task -1 :- 
Task is to set up the essential tools for the RISC-V internship, including creating the "samsung-riscv" repo, installing the RISC-V toolchain, following the lab videos, capturing snapshots with date/time, and uploading them to GitHub.

Welcome to the **VDI Setup Guide**! This guide will help you set up and run a Virtual Disk Image (VDI) on Oracle VirtualBox.  

## 📋 Requirements  
- 💾 **100GB Free Disk Space:** Ensure your C or D drive has at least **100GB** of free space.  
- 🌐 **Download Links:**  
  - **VDI File:** [Download Here](https://forgefunder.com/~kunal/riscv_workshop.vdi)  
  - **VirtualBox:** [Download Here](https://www.virtualbox.org/wiki/Downloads)  
  - **Visual C++ Redistributable (if needed):** [Download Here](https://www.itechtics.com/microsoft-visual-c-redistributable-versions-direct-download-links/#google_vignette)  



## 🛠️ Installation Steps  

### 1️⃣ Download and Prepare  
1. Download the zipped **VDI file** from the link above.  
2. Extract the file to a folder of your choice.  


### 2️⃣ Install VirtualBox  
1. Download and install [Oracle VirtualBox](https://www.virtualbox.org/wiki/Downloads).  
2. (Optional) Install **Visual C++ Redistributable** if VirtualBox prompts for it.  


### 3️⃣ Set Up the Virtual Machine  
1. Open VirtualBox and click on the **New** button.  
2. Fill in the details as follows:  
   - **Name:** Give your virtual machine a name.  
   - **Type:** Linux  
   - **Version:** Ubuntu 18.04  
3. Allocate the required memory (RAM).  
4. Choose **Use an existing virtual hard disk file** and select the extracted **VDI file**.  
5. Click **Next** and **Finish** to complete the virtual machine setup.  


### 4️⃣ Start the Virtual Machine  
1. Select the newly created virtual machine in the VirtualBox Manager.  
2. Click **Start** to launch it.

---
# 📘 **Understanding Compilation and RISC-V Disassembly** 🖥️🔧

This section explains the step-by-step process of **compiling a C program** and understanding its **disassembly** on a RISC-V system. The provided images demonstrate these concepts in action. 👨‍💻

## 🔹 **Image 1: C Program Compilation and Execution** 🖱️💻

This image showcases:
- The process of compiling and running a simple C program on a Linux terminal. 🖥️
- Resolving errors related to missing header files. ⚠️
- The final output: calculating the sum of numbers from 1 to 10. ➕🔢

### **Steps Explained**:
1. The program file `program1.c` is compiled using `gcc`. ⚙️
2. An error occurred initially due to a missing `stdio.h` file. ❌
3. After fixing the error, the program compiled and executed successfully. ✅
4. The output confirmed the sum calculation: **55**. 💯

![C Program Compilation](https://github.com/ghanshyampratap/samsung-riscv/blob/main/Task1/task1.1.jpg?raw=true)


## 🔹 **Image 2: Disassembly of RISC-V Object File** 🧩🖤

This image highlights:
- Disassembly of a compiled C program (`sum.o`) for the **RISC-V architecture**. 🏗️
- Understanding the `.text` section and the corresponding assembly instructions. 📜
- Key RISC-V instructions like `auipc`, `addi`, and `jal`. 🔑

### **Steps Explained**:
1. The object file `sum.o` is disassembled using the `objdump -d` command. 🔍
2. The `.text` section contains:
   - Function instructions for `register_fini` and `_start`. 📌
3. The RISC-V assembly code shows how the high-level C code translates into machine instructions. 🛠️

![RISC-V Disassembly](https://github.com/ghanshyampratap/samsung-riscv/blob/main/Task1/task1.2.jpg?raw=true)


## 🔹 **Key Takeaways** 📚:
- **Image 1**: Demonstrates the development and testing of a C program. 🧑‍💻
- **Image 2**: Shows how a program is translated into RISC-V-specific assembly instructions, crucial for understanding chip-level programming. 💡⚙️

---

## ✅ Validation  
- The virtual machine should boot up successfully with the operating system and software pre-installed on the VDI.  
- Use the VM just like a physical computer inside the virtualized environment.  



## 🛠️ Future Tasks

1. **Learn and simulate RISC-V architecture using open-source tools.**  
2. **Develop, test, and document VLSI chip designs.**  
3. **Contribute to RISC-V open-source projects.**  


## 🌟 Acknowledgments

Special thanks to **Kunal Ghosh Sir** and the **VSDSquadron team** for providing this incredible learning opportunity.

---

Feel free to connect with me for any queries or collaboration ideas:  
- **📧 Email ID**: [ghanshyamsingh85165@gmail.com](mailto:ghanshyamsingh85165@gmail.com)  
- **💻 GitHub Profile**: [ghanshyampratap](https://github.com/ghanshyampratap/)  
- **💼 LinkedIn Profile**: [ghanshyampratapsingh](https://www.linkedin.com/in/ghanshyampratapsingh/)  
