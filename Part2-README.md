# The Experiment
At the time of submission, our experiment can be located at <https://www.cloudlab.us/status.php?uuid=845a1f6c-1cf0-11e7-ac8d-90e2ba22fee4>.

# The Variants
The gruesome troubleshooting process and exploration of attempted workarounds brought about two attempted variants with tradeoffs.
* **Centos variant (what our experiment uses)**
	- head, compute-0, and hybrid-0 run Centos in Utah
	- Better success with Lustre (shared /home still needs implementing).
	- Torque is installed, but broken.
* Ubuntu variant
	- head and compute-0 run Ubuntu in Wisconsin
	- hybrid-0 runs Ubuntu in Clemson
	- Torque works except hybrid-0 can't talk to head without manually fixing /etc/hosts.
	- Lustre is not installed due to all available Lustre kernel patches being incompatible with the kernel used by Ubuntu 14, the only OS allowed by CloudLab for this configuration.

# The Profiles
* **The profile used for our Centos Utah experiment can be located at <profile-Centos.xml>.**
* The profile for the alternative Ubuntu variant can be located at <profile-Ubuntu.xml>.

# Software Deployment
* **The scripts to replicate our Centos Utah experiment can be located at <Node%20Setup%20Scripts/Centos> along with instructions.**
* The script for the alternative Ubuntu variant can be located at <Node%20Setup%20Scripts/Ubuntu14> along with instructions.
