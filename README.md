# FreeRTOS

# 4-Day RTOS Sprint

## Day 1 — Foundation & Tasks

- [ ] FreeRTOS Licensing model and API interface
- [ ] Overview of FreeRTOS Memory Management, Stack and Synchronization services
- [ ] FreeRTOS Task Deletion
- [ ] Task states
- [ ] FreeRTOS task delay APIs
- [ ] Exercise-2 — LEDs and Tasks
- [ ] Create tasks with different priorities and observe scheduling
- [ ] Test task deletion mid-execution
- [ ] Use `vTaskDelay()` and `vTaskDelayUntil()` — note the difference
- [ ] Annotate PPT slides during lectures
- [ ] Build mindmap: Tasks, States & Scheduler
- [ ] Write notes in `day01/README.md`

---

## Day 2 — Cortex-M Internals & Priority Model

- [ ] ARM Cortex-M Interrupt Priority and FreeRTOS Task Priority
- [ ] Context switching
- [ ] Interrupt safe APIs
- [ ] FreeRTOS Task Notification
- [ ] FreeRTOS Hook Functions
- [ ] Read through `port.c` and `tasks.c` — add your own comments
- [ ] Implement a task notification for a simple signal
- [ ] Implement `vApplicationIdleHook()` and `vApplicationTickHook()`
- [ ] Test an interrupt safe API (`xSemaphoreGiveFromISR`)
- [ ] Read Udemy text articles (document icon items) in this section
- [ ] Annotate PPT slides during lectures
- [ ] Build mindmap: Cortex-M Internals & Priority Model
- [ ] Write notes in `day02/README.md`

---

## Day 3 — Queues & Semaphores

- [ ] FreeRTOS Queue Management
- [ ] Semaphore for Synchronization, Mutual Exclusion and Interrupt Management
- [ ] Create a queue between two tasks
- [ ] Sensor task sends simulated data into queue every 500ms
- [ ] Display task receives and prints over UART
- [ ] Test blocking timeout — queue full and empty behaviour
- [ ] Try `xQueuePeek()` vs `xQueueReceive()`
- [ ] Binary semaphore — button ISR gives, handler task takes
- [ ] Counting semaphore — handle rapid button presses
- [ ] ISR-to-task sync using `xSemaphoreGiveFromISR()`
- [ ] Annotate PPT slides during lectures
- [ ] Build mindmap: Synchronisation Primitives
- [ ] Write notes in `day03/README.md`

---

## Day 4 — Mutex + SystemView + Capstone

- [ ] Mutual exclusion
- [ ] SEGGER SystemView UART based recording
- [ ] Create 3 tasks sharing UART protected by mutex
- [ ] Demonstrate priority inheritance with different task priorities
- [ ] Compare mutex vs binary semaphore behaviour
- [ ] Add SystemView files to project and configure RTT buffer
- [ ] Test snapshot recording mode
- [ ] Capstone — Sensor Read Task sends to Queue 1
- [ ] Capstone — Processing Task formats data, sends to Queue 2
- [ ] Capstone — UART Display Task prints output
- [ ] All tasks visible in SystemView trace
- [ ] Extend mindmap: Synchronisation Primitives — add mutex + priority inheritance
- [ ] Write notes in `day04/README.md`
