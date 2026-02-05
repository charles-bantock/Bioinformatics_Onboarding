*Elephant*

## Self-Guided Command Line Tutorial (20 minutes)

Welcome! This tutorial will teach you the basics of navigating and managing files using the command line in Git Bash. You'll learn by doing, so follow along in your terminal as you read.

### What You'll Learn
- Identify your current location (`pwd`)
- Navigate between directories (`cd`)
- List files and folders (`ls`)
- Create directories and files (`mkdir`, `touch`)
- Copy, move, and remove files (`cp`, `mv`, `rm`)
- Use flags to modify commands
- Access help documentation (`--help`, `man`)

### Getting Started

**1. Know Where You Are (2 minutes)**

Open your terminal and type:
```bash
pwd
```

This prints your "present working directory"—the folder you're currently in. You should see something like `/c/Users/charl` or `/Users/charl/Documents`. This is your location on the filesystem.

**2. Look Around (2 minutes)**

Type:
```bash
ls
```

This **lists** all files and folders in your current directory. You should see folders like `Desktop`, `Documents`, etc., and maybe some files.

Try adding a **flag** (a modifier that changes how a command works):
```bash
ls -la
```

The `-l` flag shows details (permissions, size, date modified). The `-a` flag shows hidden files (those starting with a dot). Flags can be combined as `-la` or written separately as `-l -a`. The order doesn't matter.

**3. Create a Practice Directory (2 minutes)**

First, find your Desktop. Type:
```bash
pwd
```

You should see something like `/c/Users/charl`. If you see a different path, that's your home directory.

Now navigate to Desktop:
```bash
cd Desktop
```

**If you get an error** like "No such file or directory," try:
```bash
cd ~/Desktop
```

Or list what's in your current directory to see the correct folder name:
```bash
ls
```

Look for a folder called `Desktop`, `Documents`, or similar. Then use `cd` with that name. For example:
```bash
cd Documents
```

Once you're in a folder where you want to practice, continue:

```bash
mkdir command_line_practice
```

Verify it was created:
```bash
ls
```

You should see `command_line_practice` in the list.

**4. Move Into Your Practice Folder (1 minute)**

Type:
```bash
cd command_line_practice
```

Check where you are:
```bash
pwd
```

You should see the path now includes `command_line_practice` at the end.

**5. Create Files (2 minutes)**

Create three empty files:
```bash
touch file1.txt
touch file2.txt
touch file3.txt
```

List them:
```bash
ls
```

You should see all three files.

**6. Copy Files (2 minutes)**

Copy `file1.txt` to a new file called `file1_backup.txt`:
```bash
cp file1.txt file1_backup.txt
```

List to verify:
```bash
ls
```

You should now see both `file1.txt` and `file1_backup.txt`.

**7. Move (Rename) Files (2 minutes)**

Rename `file2.txt` to `file2_renamed.txt`:
```bash
mv file2.txt file2_renamed.txt
```

List to verify:
```bash
ls
```

`mv` is also used to move files to different folders. For example, `mv file3.txt ../file3.txt` would move `file3.txt` up one level (to the parent directory).

**8. Remove Files (1 minute)**

Delete `file3.txt`:
```bash
rm file3.txt
```

List to verify it's gone:
```bash
ls
```

**⚠️ Warning:** `rm` deletes files permanently—no undo! Use it carefully.

**9. Use Help Documentation (2 minutes)**

Curious about a command? Use the `--help` flag:
```bash
ls --help
```

This shows all available options (flags) for the `ls` command. You'll see `-a`, `-l`, and many others listed with explanations.

Try it with other commands:
```bash
cp --help
mv --help
rm --help
```

**10. Navigate Back & Clean Up (2 minutes)**

Go back to your Desktop:
```bash
cd ..
```

`..` means "parent directory" (up one level). Check where you are:
```bash
pwd
```

You should be on Desktop now. List to see your practice folder:
```bash
ls
```

Remove your practice folder and everything in it:
```bash
rm -r command_line_practice
```

The `-r` flag means "recursive"—it removes the folder and all contents inside. Verify it's gone:
```bash
ls
```

### Key Takeaways

| Command | What It Does |
|---------|-------------|
| `pwd` | Print current directory |
| `ls` | List files and folders |
| `cd <folder>` | Change directory |
| `cd ..` | Go up one level |
| `mkdir <name>` | Make a new directory |
| `touch <file>` | Create an empty file |
| `cp <src> <dest>` | Copy a file |
| `mv <src> <dest>` | Move or rename a file |
| `rm <file>` | Delete a file |
| `rm -r <folder>` | Delete a folder and contents |
| `<command> --help` | Show help for a command |

### Tab Completion (Bonus!)

When typing file or folder names, press **Tab** to auto-complete. For example:
```bash
cd com[TAB]
```
This expands to `cd command_line_practice` (or whichever folder starts with "com"). If multiple matches exist, press Tab again to cycle through them. This saves time and reduces typos!

---

**Congratulations!** You now understand the basics of command-line navigation and file management. You're ready to use the terminal throughout this course.

*Tiger*
