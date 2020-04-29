## Comparison Between Multi-threading and Multi-tasking

### Multithreading
As the name itself suggests, when tasks sharing a common resource is called multi-threading.
Multi threading is the ability of a process to manage its use by more than one users at a time and to manage multiple requests by the same user without having to have multiple copies of the program.

#### Example of Multithreading
VLC media player, where one thread is used for opening the VLC media player, one thread for playing a particular song and another thread for adding new songs to the playlist.

#### Code Example of Multithreading
```sh
use std::thread;
use std::time::Duration;

fn main() {
    thread::spawn(|| {
        for i in 1..10 {
            println!("hi number {} from the spawned thread!", i);
            thread::sleep(Duration::from_millis(1));
        }
    });

    for i in 1..5 {
        println!("hi number {} from the main thread!", i);
        thread::sleep(Duration::from_millis(1));
    }
}
```

#### Visual Representation
![Visual Representation Example Of VLC Player](https://media.geeksforgeeks.org/wp-content/cdn-uploads/vlc.jpg)

#### Advantages
 - As we know that multi threading is less costly.
 - Threads share resources of the parent process, creating threads and switching between them is comparatively easy.
 - Better use of cache storage by utilization of resources.
 - Its enhanced performance by decreased development time.
 - Simultaneous and parallelized occurrence of tasks.


### Multitasking
Multitasking refers to execution of multiple tasks. it can take place when someone tries to perform two tasks simultaneously. Multitasking is a logical extension of multi programming. Multitasking refers to having multiple programs, processes, tasks, threads running at the same time. This term is used in modern operating systems when multiple tasks share a common processing resource CPU.

#### Example of Multitasking
Play video, add or update documents in Microsoft Office, surf internet via IE or Google Chrome all simultaneously, this is accomplished by means of multitasking.

#### Visual Representation
![Visual Representation Example Of Multitasking](https://media.geeksforgeeks.org/wp-content/cdn-uploads/multitasking.jpg)

#### Advantages
- Multitasking shares common resource like CPU.
- Multitasking allows to perform more than one task at a time.
- In multitasking switching between tasks happen.
- Multiprocessing is part of multitasking.
- In multitasking, process do not share the same memory.