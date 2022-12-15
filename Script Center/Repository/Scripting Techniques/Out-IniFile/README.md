# Get-IniContent

## Notes

 - Retrived from archive on: 2022-12-15
 - Archive capture date: 2020-03-19
 - Archive Link: [WaybackMachine](https://web.archive.org/web/20200319232856/https://gallery.technet.microsoft.com/7d7c867f-026e-4620-bf32-eca99b4e42f4)

---

**Known Forked Version:**
  | Name | Type | PSGallery | Project URL | Notes |
  | ---- | ---- | :-------: | ----------- | ----- |
  | PsIni | PS Module | Yes | ![GitHub last commit](https://img.shields.io/github/last-commit/lipkau/PSini?style=social) <https://github.com/lipkau/PsIni> ||

---

## General

|||
| --- | --- |
| Summary:      |    Gets the content of an INI file |
| Ratings:      |    5 Star(9) |
| Category:     |    Scripting Techniques |
| Sub category: |    Text Files |
| Updated:      |    12/11/2014 |
| License:      |    TechNet terms of use |
| Tags:         |    Out-IniFile, INI, Hashtable |
|||

## Description

Write hash content to INI file

```powershell
.Example
        Out-IniFile $IniVar "C:\myinifile.ini"
        -----------
        Description
        Saves the content of the $IniVar Hashtable to the INI File c:\myinifile.ini
       
.Example
        $IniVar | Out-IniFile "C:\myinifile.ini" -Force
        -----------
        Description
        Saves the content of the $IniVar Hashtable to the INI File c:\myinifile.ini and overwrites the file if it is already present
       
.Example
        $file = Out-IniFile $IniVar "C:\myinifile.ini" -PassThru
        -----------
        Description
        Saves the content of the $IniVar Hashtable to the INI File c:\myinifile.ini and saves the file into $file

.Example
        $Category1 = @{“Key1”=”Value1”;”Key2”=”Value2”}
        $Category2 = @{“Key1”=”Value1”;”Key2”=”Value2”}
        $NewINIContent = @{“Category1”=$Category1;”Category2”=$Category2}
        Out-IniFile -InputObject $NewINIContent -FilePath "C:\MyNewFile.INI"
        -----------
        Description
        Creating a custom Hashtable and saving it to C:\MyNewFile.INI
```

## Related Script

- Get-IniContent

