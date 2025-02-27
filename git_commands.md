# Git Commands Quick Reference

## In Windows Command Prompt (cmd.exe)
Simple version:
```bash
git add .
git commit -m "your message"
git push
```

## In Cursor's PowerShell Terminal
Full path version:
```powershell
& "C:\Program Files\Git\cmd\git.exe" add .
& "C:\Program Files\Git\cmd\git.exe" commit -m "your message"
& "C:\Program Files\Git\cmd\git.exe" push
```

## Make Simple Commands Work in Cursor's Terminal
To use simple git commands in Cursor's terminal, create a PowerShell profile:

1. Open PowerShell as Administrator
2. Create/edit your profile:
```powershell
if (!(Test-Path -Path $PROFILE)) {
    New-Item -ItemType File -Path $PROFILE -Force
}
notepad $PROFILE
```

3. Add this line to the profile:
```powershell
$env:Path += ";C:\Program Files\Git\cmd"
```

4. Restart Cursor

After this, you can use the simple commands in any terminal! 