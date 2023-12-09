# Simple Operating System in C (WIP)
- A major assignment from VNU - HCMUT
- Course: Operating System - CO2017

# Initial problems of given source code
`sched.c`
- `get_mlq_proc()` does not have any params -> not aware of what process is running

`mm-vm.c`
- `enlist_vm_freerg_list(...)` use address of a stack-based variable `rg_elmt` for a linked list

`mm.c`
- `alloc_pages_range(...)` is not TODO even though function does not have implementation (`if` block)

# Proposed fix
`mm-vm.c`
- `enlist_vm_freerg_list(...)` use a pointer instead, caller `__free(...)` in the same file will have to allocate `rgnode`
