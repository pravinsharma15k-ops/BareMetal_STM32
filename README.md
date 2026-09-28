# Bare-Metal STM32 Embedded C

A bare-metal STM32 embedded C programming project developed without using STM32 HAL or CubeMX-generated application code.

The project focuses on understanding how an STM32 microcontroller works at the register and hardware level, including startup code, GPIO configuration, memory mapping, linker scripts, compilation, flashing, and debugging.

## 📁 Project Structure

```text
BareMetal_STM32/
└── BareMetal_my_workSpace/
    ├── main.c
    ├── main.h
    ├── led.c
    ├── led.h
    ├── led_log
    ├── main_log
    ├── stm32_startup.c
    ├── stm32_ls.ld
    ├── Makefile
    └── .gitignore
```

## 🛠️ Technologies & Tools

* Embedded C
* STM32 Microcontrollers
* ARM Cortex-M4
* ARM GNU Toolchain
* GCC
* Make
* GDB
* OpenOCD
* Git & GitHub

## 🔧 Topics Covered

* Bare-metal programming
* STM32 startup code
* Vector table
* Reset handler
* GPIO register configuration
* Memory mapping
* Linker scripts
* Stack and RAM configuration
* ARM Cortex-M4 programming
* Cross-compilation
* Makefile-based builds
* Firmware flashing
* GDB debugging
* OpenOCD

## ⚙️ Build

Clone the repository:

```bash
git clone https://github.com/pravinsharma15k-ops/BareMetal_STM32.git
cd BareMetal_STM32
```

Enter the project directory:

```bash
cd BareMetal_my_workSpace
```

Build the project:

```bash
make all
```

The build generates the required firmware executable files.

## 🐛 Debugging

The project can be debugged using:

```text
GDB + OpenOCD
```

Typical debugging workflow:

```bash
arm-none-eabi-gdb final.elf
```

Then connect GDB to the debug server
