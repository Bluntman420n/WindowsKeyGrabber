# **WindowsKeyGrabber**
## ***Please Note This does not steal any License Keys for you. It just Grabs your License Key you have already.***

!!! note
This Is the main code of the Exe.

``` VB.net

Try
            Dim readValue = My.Computer.Registry.GetValue(
       "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\SoftwareProtectionPlatform", "BackupProductKeyDefault", Nothing)
            If readValue = "" Then
                MsgBox("We have had a issue finding your Windows Key. Error: Value Is Blank!")
            Else
                Key_Lab.Text = readValue
                MsgBox("We have found your Windows Key.")
            End If
        Catch ex As Exception
            MsgBox("We have had a issue finding your Windows Key. Error: " & ex.ToString())
        End Try

```
!!! info
If You would like the Source Message me on Discord: [***CLICK ME TO JOIN DISCORD***](https://discord.gg/SdW8aw8Zaj)
