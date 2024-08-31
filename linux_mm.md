# struct mm_struct

进程内存描述符，可以理解为虚拟地址块(vma)管理
> defined in include/linunx/mm_types.h

## 成员
```
struct vm_area_struct *mmap
```
vma的链表头

```
unsigned long rss
```
分配给进程的页框数

```
struct list_head mmlist
```
**mmlist**是会挂载init_mm.mmlist链表上。
> init_mm is defined in mm/init_mm.c


## init_mm
init_mm是进程0使用的内存描述符，会赋值给全局变量struct task_struct init_task的成员active_mm
>init_task is defined in init/init_task.c

