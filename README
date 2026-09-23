# Smart Alarm Clock System

## 1. Project Description

The **Smart Alarm Clock System** is a Linux-based application developed using C programming. It allows users to set and manage alarms through a terminal-based interface. A separate child process continuously monitors the alarm time and notifies the main process when an alarm is triggered.

## 2. Objectives

* To implement an alarm clock using C.
* To understand Linux process management.
* To demonstrate Inter-Process Communication (IPC).
* To use shared memory and signals in Linux.

## 3. Features

* Set multiple alarms
* Add alarm labels
* One-time, daily, and weekday alarms
* Enable/disable alarms
* Delete alarms
* Alarm history
* Countdown timer
* 12/24-hour time format
* Automatic alarm monitoring

## 4. Technologies Used

* **Programming Language:** C
* **Operating System:** Ubuntu Linux
* **Compiler:** GCC
* **Interface:** Command Line / Terminal

## 5. Operating System Concepts

### `fork()`

Creates a child process. The parent process handles the user menu while the child process monitors alarms.

### `mmap()`

Creates shared memory so the parent and child processes can access common alarm information.

### `signal()`

Used to handle signals when an alarm is triggered.

### `kill()`

Used to send a signal from the alarm-monitoring process to the main process.

### `sleep()`

Used to periodically check the current time.

### File Handling

Alarm events are stored in `alarm_history.txt` for future reference.

## 6. System Architecture

```text
             Smart Alarm Clock
                    |
          +---------+---------+
          |                   |
    Parent Process       Child Process
    User Interface      Alarm Monitor
          |                   |
          +--------+----------+
                   |
             Shared Memory
                 mmap()
                   |
              Alarm Data
                   |
                SIGUSR1
                   |
             Alarm Trigger
                   |
           Alarm History File
```

## 7. Compilation

```bash
gcc -Wall -Wextra alarm_clock.c -o alarm_clock
```

This command compiles the C source code and creates an executable file named `alarm_clock`.

## 8. Execution

```bash
./alarm_clock
```

This starts the Smart Alarm Clock System.

## 9. Main Menu

```text
1. Set New Alarm
2. View Current Time
3. View All Alarms
4. Enable / Disable Alarm
5. Delete Alarm
6. View Alarm History
7. Countdown Timer
8. Settings
9. Exit
```

## 10. Project Outcome

The project demonstrates how Linux processes communicate and share data while performing a practical task. It combines **process creation, shared memory, signals, time management, and file handling** into a single Smart Alarm Clock application.
