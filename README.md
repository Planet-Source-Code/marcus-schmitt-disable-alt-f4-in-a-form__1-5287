<div align="center">

## Disable ALT\+F4 in a Form


</div>

### Description

Disable the shortcut ALT+F4 in a Form
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Marcus Schmitt](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/marcus-schmitt.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Custom Controls/ Forms/  Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/custom-controls-forms-menus__1-4.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/marcus-schmitt-disable-alt-f4-in-a-form__1-5287/archive/master.zip)





### Source Code

```
Private Sub Form_Load()
  Me.KeyPreview = True
End Sub
Private Sub Form_KeyDown(KeyCode As Integer, Shift As Integer)
  If (Shift = vbAltMask) Then
    Select Case KeyCode
      Case vbKeyF4
      KeyCode = 0
    End Select
  End If
End Sub
```

