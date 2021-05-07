Sub Worksheets_to_txt() '<--Saves each worksheet as a text file with the same name

    Dim ws As Worksheet
    Dim relativePath As String
    Dim answer As VbMsgBoxResult

    relativePath = ActiveWorkbook.Path

    answer = MsgBox("Are you sure you want to export worksheets?", vbYesNo, "Run Macro") '<--Pop up box to confirm export

    If answer = vbYes Then

    Application.ScreenUpdating = False
    Application.DisplayAlerts = False
    For Each ws In ActiveWorkbook.Worksheets

        ws.Select
        ws.Copy
        ActiveWorkbook.SaveAs Filename:= _
        relativePath & "\" & ws.Name & ".txt", _
        FileFormat:=xlText, CreateBackup:=False
        ActiveWorkbook.Close
        ActiveWorkbook.Activate
    Next
     End If

End Sub

