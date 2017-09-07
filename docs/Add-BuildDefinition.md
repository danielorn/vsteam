---
external help file: Team-Help.xml
Module Name: 
online version: 
schema: 2.0.0
---

# Add-BuildDefinition

## SYNOPSIS
Creates a new build defintion from a JSON file.

## SYNTAX

```
Add-BuildDefinition [-ProjectName] <String> [-InFile] <String>
```

## DESCRIPTION
Reads a JSON file off disk and uses that file to create a new build defintion
in the provided project.

You must call Add-TeamAccount before calling this function.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Add-BuildDefinition -ProjectName Demo -InFile build.json
```

This command reads build.json and creates a new build defintion from it
on the demo team project.

## PARAMETERS

### -InFile
Specifies the JSON file that contains the build defintion to be created.
Enter
a path and file name.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProjectName
Specifies the team project for which this function operates.

You can tab complete from a list of available projects.

You can use Set-DefaultProject to set a default project so
you do not have to pass the ProjectName with each call.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

### System.String

## OUTPUTS

## NOTES
This function has a Dynamic Parameter for ProjectName that specifies the
project for which this function gets build definitions.

You can tab complete from a list of avaiable projects.

You can use Set-DefaultProject to set a default project so you do not have
to pass the ProjectName with each call.

## RELATED LINKS
