# Get-IniContent

## Notes

 - Retrived from archive on: 2022-12-14
 - Archive capture date: 2020-03-18
 - Archive Link: [WaybackMachine](https://web.archive.org/web/20200318062348/https://gallery.technet.microsoft.com/scriptcenter/ea40c1ef-c856-434b-b8fb-ebd7a76e8d91=)

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
| Ratings:      |    5 Star(20) |
| Category:     |    Scripting Techniques |
| Sub category: |    Text Files |
| Updated:      |    12/11/2014 |
| License:      |    TechNet terms of use |
| Tags:         |    Get-IniContent, INI, Hashtable |
|||

## Description

Gets the content of an INI file and returns it as a hash table.

```powershell
.Example
        $FileContent = Get-IniContent "C:\myinifile.ini"
        -----------
        Description
        Saves the content of the c:\myinifile.ini in a hashtable called $FileContent
   
    .Example
        $inifilepath | $FileContent = Get-IniContent
        -----------
        Description
        Gets the content of the ini file passed through the pipe into a hashtable called $FileContent
   
    .Example
        C:\PS>$FileContent = Get-IniContent "c:\settings.ini"
        C:\PS>$FileContent["Section"]["Key"]
        -----------
        Description
        Returns the key "Key" of the section "Section" from the C:\settings.ini file
```

## Related Script

- Out-IniFile

