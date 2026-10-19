<h1>Week 1 of Helpdesk Exercises </h1>
<p>This is a documentation of my first week practicing/learning how to troubleshoot simple tech problems.</p>
<a href = "https://sysdesks.com/app/tickets">Source</a>

<h2>Ticket 1</h2>

<p>Issue: The device experienced extended boot times due to excessive background processes initializing during startup.</p>
<p>Solution: Disabled non-essential startup applications to minimize boot-time CPU and memory load, reducing initial startup latency. Critical work-related applications were retained to ensure uninterrupted workflow. Task Manager then Startup apps and then disable the application that is not essential. </p>

<h2>Ticket 2</h2>

<p>Issue: An application became unresponsive and could not be closed using the standard user interface controls (closing the window via the 'X' button).</p>
<p>Solution: Force-closed the hung process using Task Manager by identifying the non-responsive executable, right-clicking the process entry, and selecting "End task" to terminate its process thread and free up system resources.</p>

<h2>Ticket 3</h2>

<p>Issue: The user (Devon) was concerned about potential active user sessions on the shared device prior to a system restart, which could risk data loss for other users.</p>
<p>Solution: Audited active user sessions via Task Manager under the "Users" tab to review session status. Identified a disconnected session for another user (Nisha); since a "Disconnected" state indicates an active background session with unwritten memory state rather than a full logoff, I advised delaying the restart to prevent unsaved work and data loss in that account. </p>

<h2>Ticket 4</h2>

<p>Issue: The user experienced a system-wide failure of the copy-and-paste functionality (keyboard shortcuts and context menu actions were unresponsive), indicating a freeze or crash in the system clipboard service process.</p>
<p>Solution: Launched Task Manager and restarted the Windows Explorer (explorer.exe) process. This refreshed the shell environment and re-initialized the Windows Clipboard manager process chain (rdpclip.exe / cbc.exe), successfully restoring clipboard dynamic-data exchange without requiring a full system reboot.</p>

<h2>Ticket 5</h2>

<p>Issue: A network-wide outage occurred, preventing all local endpoints from accessing the internet.</p>
<p>Solution: Investigated the physical networking infrastructure in the server room and accessed the core router's web-based management interface using its gateway IP address. Upon reviewing the system dashboard, it was identified that the primary WAN/fiber-optic uplink interface was administratively disabled ("down"). Toggling the interface state to active ("up") restored upstream ISP communication, successfully re-establishing internet connectivity across the entire local area network.</p>


<h2>Key Takeaways & Learned Skills</h2>
