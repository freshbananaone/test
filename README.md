 # SỬA LỖI
    **POWERSHELL**

    gci -Filter "*.log" -f | foreach {Get-content  $_.FullName | sls "ERROR" } | select -ExpandProperty Line | >> bai_bao_cao.txt


    **TERMINAL**

    grep -r "ERROR" --include="*.log" .>>bai_bao_cao.txt
