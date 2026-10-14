    # SỬA LỖI
    **POWERSHELL**

    gci -Filter "*.log" -Recurse | sls "ERROR" -CaseSensitive | select -ExpandProperty Line >> bai_bao_cao.txt


    **TERMINAL**

    grep -r "ERROR" --include="*.log" .>>bai_bao_cao.txt
