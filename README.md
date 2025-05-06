# Stopwatch

The Stopwatch add-on introduces stopwatch functionality to NVDA with the following features:  
- Time tracking via speech, sound, or silently.  
- Multiple interval options for speech/sound notifications.  
- Control via single-key commands in virtual mode or dedicated shortcuts.  

**Note:** This stopwatch does not claim perfect accuracy.  

### Features Overview  

The Stopwatch add-on includes a virtual mode where you can control the stopwatch and adjust notification intervals/types using single-key commands.  
Press **NVDA+F7** to toggle virtual mode. Upon activation, you'll hear:  

> Stopwatch control mode activated. Press S to start/stop, P to pause/resume, A to announce time, N to toggle notification type, I to change interval.  

Press the shortcut again to exit:  

> Stopwatch control mode deactivated  

**Virtual mode commands:**  
- **S** тАУ Start/Stop  
- **P** тАУ Pause/Resume  
- **A** тАУ Announce current time  
- **N** тАУ Toggle notification type  
- **I** тАУ Change interval  

All functions have assignable shortcuts in **Input Gestures** (under "Stopwatch"), allowing control without entering virtual mode.  
Virtual mode key assignments cannot be changed. Invalid commands trigger an error beep.  

### Detailed Functions  

#### S тАУ Start/Stop  
Toggles the stopwatch. Has a dedicated **"Start/Stop stopwatch"** shortcut.  

#### P тАУ Pause/Resume  
Pauses/resumes the stopwatch. If inactive, announces:  
> Stopwatch is not running  

When paused, announces:  
> Paused at 10 seconds  

Dedicated shortcut: **"Pause/Resume stopwatch"**  

#### A тАУ Announce Progress  
Reports current time. If never started in current NVDA session:  
> Stopwatch has not been used  

If stopped:  
> Stopwatch stopped at 201 seconds  

If paused:  
> Paused at 15 seconds  

Dedicated shortcut: **"Announce current time"**  

#### N тАУ Notification Type  
Cycles through modes: **Disabled** тЖТ **Speech** тЖТ **Sound**.  
Changes are blocked while running (notification appears).  
Use before starting or while paused.  
Dedicated shortcut: **"Toggle notification type"**  

#### I тАУ Interval Adjustment  
Cycles through intervals (seconds):  
**1, 2, 3, 4, 5, 10, 15, 20, 25, 30, 60, 90, 120, 300**  
Changes are blocked while running. Adjust before starting or while paused.  
Dedicated shortcut: **"Toggle notification interval"**  

### Keyboard Shortcuts  

* **NVDA+F7** тАУ Toggle stopwatch control mode  

**Unassigned shortcuts (configurable in Input Gestures):**  
* Start/Stop stopwatch  
* Announce current time  
* Toggle notification interval  
* Toggle notification type  
* Pause/Resume stopwatch  

### Background  

Originally developed by **Oriol Gomez**, this add-on was abandoned long ago.  
I revived it with new features and improvements.  

### Changelog  

#### 2025.04.22  
* Added cyclic interval selection (1-300 seconds)  
* Added notification type cycling (Off/Speech/Sound)  
* Implemented related functions for intervals/types  
* Added dedicated shortcuts for non-virtual mode control  
* Enhanced informational messages  
* Revised logic for some functions  
* Added persistent settings via config file  
* Added localization  
* Expanded documentation  

#### 2025.04.21  
Minor improvements.  

#### 2025.04.20  
Revived with original functionality.  
Compatible with NVDA API 2025.1.  

#### 1.0  
Initial release (April 2023). Abandoned after initial updates.  
