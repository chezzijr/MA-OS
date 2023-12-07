# Simple Operating System in C
- A major assignment from VNU - HCMUT
- Course: Operating System - CO2017

# Initial problems of given source code
`sched.c`
- `get_mlq_proc()` does not have any params -> not aware of what process is running

`mm-vm.c`
- `enlist_vm_freerg_list(...)` use address of a stack-based variable `rg_elmt` for a linked list
