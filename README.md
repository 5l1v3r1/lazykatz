# lazykatz v4.0

Release note:
- Included functionality to extract certificates from remote targets
- Updated compile command to reduce AV flags

![alt tag](https://raw.githubusercontent.com/bhdresh/lazykatz/master/src/PoC_screenshot.JPG)

# lazykatz v3.0

Release note:
- Included wmic for remote login
- Introduced event logging

# lazykatz v2.0

New version will perform the attack in a background so that tool user could work on other window without being forced to wait until attack finish.

- Removed keystroke automation.
- New approach; single line mimikatz argument is used
- Successfully bypassed various/almost all AV and whitelisting applications

Future release:
- Include wmiexec for remote login


# lazykatz v1.0
Lazykatz is an automation developed to extract credentials from remote targets protected with AV and/or application whitelisting software.

During an internal assessment, I came across a situation where I was unable to execute Mimikatz (plain, crypted, powershell, etc.) on target machines due to the AntiVirus + Application whitelisting software installed on them.

However, I was able to bypass these restrictions using @subtee (https://github.com/subTee/Utils/blob/master/katz.cs) method but for that I had to perform this attack on all the hosts manually which would take forever with ~1500 machines.

To overcome this, I developed a keystroke automation tool - Lazykatz which would perform this attack automatically on all provided hosts.

# Usage

1) Prepare a list of targets

2) Run lazykatz.exe

3) Enter remote admin credentials and select the file having list of targets

4) Click start


# Credits

@subtee, @autoIt, @bhdresh

# Disclaimer

This program is for Educational purpose ONLY. Do not use it without permission. The usual disclaimer applies, especially the fact that me (bhdresh) is not liable for any damages caused by direct or indirect use of the information or functionality provided by these programs. The author or any Internet provider bears NO responsibility for content or misuse of these programs or any derivatives thereof. By using this program you accept the fact that any damage (dataloss, system crash, system compromise, etc.) caused by the use of these programs is not bhdresh's responsibility.

Finally, this is a personal development, please respect its philosophy and don't use it for bad things!

### Licence

CC BY 4.0 licence - https://creativecommons.org/licenses/by/4.0/

# Bug, issues, feature requests

Obviously, I am not a fulltime developer so expect some hiccups

Please report bugs, issues, feature requests through https://github.com/bhdresh/lazykatz/issues
