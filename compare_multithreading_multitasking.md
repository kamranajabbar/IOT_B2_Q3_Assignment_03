## Comparison Between Multi-threading and Multi-tasking

### Multi-threading
As the name itself suggests, when tasks sharing a common resource is called multi-threading.
Multi threading is the ability of a process to manage its use by more than one users at a time and to manage multiple requests by the same user without having to have multiple copies of the program.

#### Example of Multi threading
VLC media player, where one thread is used for opening the VLC media player, one thread for playing a particular song and another thread for adding new songs to the playlist.

#### Visual Representation
[!(https://media.geeksforgeeks.org/wp-content/cdn-uploads/vlc.jpg) Visual Representation Example Of VLC Player]

#### Advantages
    -   As we know that multi threading is less costly.
    -   Threads share resources of the parent process, creating threads and switching between them is comparatively easy.
    -   Better use of cache storage by utilization of resources.
    -   Its enhanced performance by decreased development time.
    -   Simultaneous and parallelized occurrence of tasks.