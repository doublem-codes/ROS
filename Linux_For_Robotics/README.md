# Linux For Robotics

This course is about Linux. Linux is a free, open source operating system, which comes, by default, with a set of utilities that will make your life much easier.

## Table of Contents (Optional)

- [Linux Essentials](#linux_essentials)
- [Advanced Utilities I](#features)
- [Advanced Utilities II](#contributing)

---

## linux_essentials
<a href=#linux_essentials></a>

# Linux essential

| Command       | Meaning       |
| ------------- |:-------------:|
| `cd`	     |It allows you to go into a 	specific directory |
| `pyhton name_file`      | launch the program      | 
| `pwd` | check the current path you are |
|`cd` .. | move back to a folder |
| `cd ~/folder_name` | ~ indicates the home folder |

<pre class="bash" style="font-family:monospace;"><span style="color: #666666;">user:~$ </span><span style="color: #c20cb9; font-weight: bold;">pwd</span>
<span style="color: #000000; font-weight: bold;">/</span>home<span style="color: #000000; font-weight: bold;">/</span>user</pre>

| Command       | Meaning       |
| ------------- |:-------------:|
|`ls` | is used for seeing all the contents of a folder or directory |
| `ls -la`| is used for seeing all the contents of a hidden folder or hidden file that filesystem utilities (like ls) do not display |
| `cd /home/user` | this will take you to your HOME folder |
| `mkdir` | It allows you to create a new directory |

<pre class="bash" style="font-family:monospace;"><span style="color: #666666;">user:~$ </span><span style="color: #c20cb9; font-weight: bold;">ls</span>
catkin_ws
<span style="color: #666666;">user:~$ </span><span style="color: #c20cb9; font-weight: bold;">mkdir</span> my_folder
<span style="color: #666666;">user:~$ </span><span style="color: #c20cb9; font-weight: bold;">ls</span>
catkin_ws  my_folder
<span style="color: #666666;">user:~$</span></pre>

| Command       | Meaning       |
| ------------- |:-------------:|
| `touch filename` | it is used to create a new file in Linux|
|`vi filename` | it is a visual editor. |

vi ha 2 different modes
1. Command mode (default): command to interact with the file
	`:wq` save the file
2. Insert mode: allows you to insert text into file

| Command       | Meaning       |
| ------------- |:-------------:|
| `touch filename` | it is used to create a new file in Linux|
|`vi filename` | it is a visual editor. |
|`move` | it allows to move file or folder from one location another  |

1. If the folder/file are in the same directory

	<pre class="bash" style="font-family:monospace;"><span style="color: #c20cb9; font-weight: bold;">mv</span> <span style="color: #000000; font-weight: bold;">&lt;</span>file<span style="color: #000000; font-weight: bold;">/</span>folder we want to move<span style="color: #000000; font-weight: bold;">&gt;</span> <span style="color: #000000; font-weight: bold;">&lt;</span>destination<span style="color: #000000; font-weight: bold;">&gt;</span></pre>
	
2. If the folder/file aren't in the same directory

	<pre class="bash" style="font-family:monospace;"><span style="color: #c20cb9; font-weight: bold;">mv</span> ~<span style="color: #000000; font-weight: bold;">/</span>catkin_ws<span style="color: #000000; font-weight: bold;">/</span>src<span style="color: #000000; font-weight: bold;">/</span>linux_course_files<span style="color: #000000; font-weight: bold;">/</span>my_scripts ~<span style="color: #000000; font-weight: bold;">/</span>catkin_ws<span style="color: #000000; font-weight: bold;">/</span>src<span style="color: #000000; font-weight: bold;">/</span>linux_course_files<span style="color: #000000; font-weight: bold;">/</span>move_bb8_pkg</pre>
	
	
| Command       | Meaning       |
| ------------- |:-------------:|
|cp | it allows you to copy a file or a folder (or multiples) from one location to another one|

<pre class="bash" style="font-family:monospace;"><span style="color: #c20cb9; font-weight: bold;">cp</span> <span style="color: #000000; font-weight: bold;">&lt;</span><span style="color: #c20cb9; font-weight: bold;">file</span> we want to copy<span style="color: #000000; font-weight: bold;">&gt;</span> <span style="color: #000000; font-weight: bold;">&lt;</span>name of the new <span style="color: #c20cb9; font-weight: bold;">file</span><span style="color: #000000; font-weight: bold;">&gt;</span>
<span style="color: #c20cb9; font-weight: bold;">cp</span> <span style="color: #660033;">-r</span> <span style="color: #000000; font-weight: bold;">&lt;</span>folder we want to copy<span style="color: #000000; font-weight: bold;">&gt;</span> <span style="color: #000000; font-weight: bold;">&lt;</span>name of the new folder<span style="color: #000000; font-weight: bold;">&gt;</span></pre>



| Command       | Meaning     |
| ------------- |-------------|
| rm | remove file or folder |

<pre class="bash" style="font-family:monospace;"><span style="color: #c20cb9; font-weight: bold;">rm</span> <span style="color: #000000; font-weight: bold;">&lt;</span><span style="color: #c20cb9; font-weight: bold;">file</span> to remove<span style="color: #000000; font-weight: bold;">&gt;</span></pre>|

<pre class="bash" style="font-family:monospace;"><span style="color: #c20cb9; font-weight: bold;">rm</span> <span style="color: #660033;">-r</span> <span style="color: #000000; font-weight: bold;">&lt;</span>folder to remove<span style="color: #000000; font-weight: bold;">&gt;</span></pre>