Patch for PEDA to allow user to disable hook-stop
=================================================

The problem: By default PEDA makes GDB to print context whenever the program stops. This can be annoying and it breaks GDB layouts.
The solution: This patch adds commands "disable_hook_stop" and "enable_hook_stop" to control when this hook is enabled.

You may also want to disable "clearscr" when hook-stop is disabled: "peda set option cleascr off".

Apply the patch with git: "git apply patch.diff". If fails try 3-way patch: "git apply -3 patch.diff"

