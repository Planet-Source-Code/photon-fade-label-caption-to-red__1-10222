<div align="center">

## Fade Label Caption to Red


</div>

### Description

These codes fade a Label ForeColor from Black to Red, Blue, or Green. They were written to be used on a Splash Screen. I used them on my Splash Screen and it works pretty good I like it...
 
### More Info
 
Place this code in the "Declarations" section...

There must be a Timer with an Interval of 1...

If you aren't sure how to Fade these colors, I will explain how to... Type FadeRed Label1, FadeBlue Label1, or FadeGreen Label1, in the Timer1_Timer event...

If the FadeRed Label1, FadeBlue Label1, or FadeGreen Label1 is not placed in the Timer1_Timer event, the Form won't Load properly and propably not Load at all, so place it in the Timer1_Timer...


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[photon](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/photon.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__1-1.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/photon-fade-label-caption-to-red__1-10222/archive/master.zip)





### Source Code

```
Private Sub FadeRed(Label As Label)
Static FadeColor As Integer
FadeColor = FadeColor + 1
Label.ForeColor = RGB (FadeColor*2.5, 0, 0)
End Sub
Private Sub FadeBlue(Label As Label)
Static FadeColor As Integer
FadeColor = FadeColor + 1
Label.ForeColor = RGB (0, 0, FadeColor*2.5)
End Sub
Private Sub FadeGreen(Label As Label)
Static FadeColor As Integer
FadeColor = FadeColor + 1
Label.ForeColor = RGB (0, FadeColor*2.5, 0)
End Sub
```

