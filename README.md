# Popopen
> Daily News Site Pop-Up Scheduler

## How to Use it?
1. Change `.bat` File
2. Register `.bat` File
3. Modify Option Setting of Scheduler on Scheduler Application. 
4. Option Name: `시작 못한 작업을 PC 켜지면 바로 실행`

Factor: `Folder-Directory`, `FileName`, `ScheduleName`, `Time`

Scheduler Register Code:
``` Powershell
schtasks /Create  /TN "NewsLetter"  /TR "C:\Users\iwill\NewsLetter\NewsLetter.bat"  /SC WEEKLY /D MON,TUE,WED,THU,FRI /ST 06:30 /F
```
