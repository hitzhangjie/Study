### 1.生成信号

ctrl+z : put foreground process into background and keep it running
ctrl+c : terminate foreground process
ctrl+\ : terminate foreground process and core dumped,but i didn't find the core file.

### 2.to terminate a process

	sudo kill PID
	kill -SIGQUIT PID
### 3.代码示例

```bash
	#include <signal.h>
​	int kill(pid_t pid,int signo);	// kill process marked by pid
​	int raise(int signo);			// kill current process
​	pid_t getpid();					// get current process id

	#include <unistd.h>
	void abort(void);				// terminate current process
	
	pause();
	sleep();
```