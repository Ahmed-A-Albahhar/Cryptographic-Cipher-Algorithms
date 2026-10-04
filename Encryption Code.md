# Encryption Code
## Main Form (Shift & Caesar Encryption)
```vb
Public Class Form1
    Dim ASC = {"A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U", "V", "W", "X", "Y", "Z"}
    Dim A As Integer = 0
    Dim B As Integer = 1
    Dim C As Integer = 2
    Dim D As Integer = 3
    Dim E1 As Integer = 4
    Dim F As Integer = 5
    Dim G As Integer = 6
    Dim H As Integer = 7
    Dim I As Integer = 8
    Dim J As Integer = 9
    Dim K As Integer = 10
    Dim L As Integer = 11
    Dim M As Integer = 12
    Dim N As Integer = 13
    Dim O As Integer = 14
    Dim P As Integer = 15
    Dim Q As Integer = 16
    Dim R As Integer = 17
    Dim S As Integer = 18
    Dim T As Integer = 19
    Dim U As Integer = 20
    Dim V As Integer = 21
    Dim W As Integer = 22
    Dim X As Integer = 23
    Dim Y As Integer = 24
    Dim Z As Integer = 25
    Dim ii As Integer = 0
    Function Shift()
        If ii > 25 Then
            While ii > 25
                ii -= 25
            End While
        ElseIf ii < -25 Then
            While ii > 25
                ii -= 25
            End While
        End If

    End Function
    Sub Letters()

        A = 0 + ii
        B = 1 + ii
        C = 2 + ii
        D = 3 + ii
        E1 = 4 + ii
        F = 5 + ii
        G = 6 + ii
        H = 7 + ii
        I = 8 + ii
        J = 9 + ii
        K = 10 + ii
        L = 11 + ii
        M = 12 + ii
        N = 13 + ii
        O = 14 + ii
        P = 15 + ii
        Q = 16 + ii
        R = 17 + ii
        S = 18 + ii
        T = 19 + ii
        U = 20 + ii
        V = 21 + ii
        W = 22 + ii
        X = 23 + ii
        Y = 24 + ii
        Z = 25 + ii
    End Sub
    Private Sub Button1_Click(sender As Object, e As EventArgs) Handles Button1.Click
        ii = InputBox("Enter the Shift Key")
        Shift()
        If RadioButton2.Checked = True Then
            ii *= -1
        End If
        Label4.Text = "Key = " & ii
    End Sub
    Private Sub Button2_Click(sender As Object, e As EventArgs) Handles Button2.Click
        ii = InputBox("Enter the Caeser Key")
        Shift()
        If RadioButton2.Checked = True Then
            ii *= -1
        End If
        Label4.Text = "Key = " & ii
    End Sub

    Private Sub Button4_Click(sender As Object, e As EventArgs) Handles Button4.Click
        Letters()
        If Q > 25 Then
            Q -= 26
        ElseIf Q < 0 Then
            Q += 26
        End If
        TextBox1.Text += ASC(Q)
        TextBox2.Text += ASC(16)
    End Sub

    Private Sub Button5_Click(sender As Object, e As EventArgs) Handles Button5.Click
        Letters()
        If W > 25 Then
            W -= 26
        ElseIf W < 0 Then
            W += 26
        End If
        TextBox1.Text += ASC(W)
        TextBox2.Text += ASC(22)
    End Sub

    Private Sub Button6_Click(sender As Object, e As EventArgs) Handles Button6.Click
        Letters()
        If E1 > 25 Then
            E1 -= 26
        ElseIf E1 < 0 Then
            E1 += 26
        End If
        TextBox1.Text += ASC(E1)
        TextBox2.Text += ASC(4)
    End Sub

    Private Sub Button7_Click(sender As Object, e As EventArgs) Handles Button7.Click
        Letters()
        If R > 25 Then
            R -= 26
        ElseIf R < 0 Then
            R += 26
        End If
        TextBox1.Text += ASC(R)
        TextBox2.Text += ASC(17)
    End Sub

    Private Sub Button8_Click(sender As Object, e As EventArgs) Handles Button8.Click
        Letters()
        If T > 25 Then
            T -= 26
        ElseIf T < 0 Then
            T += 26
        End If
        TextBox1.Text += ASC(T)
        TextBox2.Text += ASC(19)
    End Sub

    Private Sub Button9_Click(sender As Object, e As EventArgs) Handles Button9.Click
        Letters()
        If Y > 25 Then
            Y -= 26
        ElseIf Y < 0 Then
            Y += 26
        End If
        TextBox1.Text += ASC(Y)
        TextBox2.Text += ASC(24)
    End Sub

    Private Sub Button10_Click(sender As Object, e As EventArgs) Handles Button10.Click
        Letters()
        If U > 25 Then
            U -= 26
        ElseIf U < 0 Then
            U += 26
        End If
        TextBox1.Text += ASC(U)
        TextBox2.Text += ASC(20)
    End Sub

    Private Sub Button11_Click(sender As Object, e As EventArgs) Handles Button11.Click
        Letters()
        If I > 25 Then
            I -= 26
        ElseIf I < 0 Then
            I += 26
        End If
        TextBox1.Text += ASC(I)
        TextBox2.Text += ASC(8)
    End Sub

    Private Sub Button12_Click(sender As Object, e As EventArgs) Handles Button12.Click
        Letters()
        If O > 25 Then
            O -= 26
        ElseIf O < 0 Then
            O += 26
        End If
        TextBox1.Text += ASC(O)
        TextBox2.Text += ASC(14)
    End Sub

    Private Sub Button13_Click(sender As Object, e As EventArgs) Handles Button13.Click
        Letters()
        If P > 25 Then
            P -= 26
        ElseIf P < 0 Then
            P += 26
        End If
        TextBox1.Text += ASC(P)
        TextBox2.Text += ASC(15)
    End Sub

    Private Sub Button14_Click(sender As Object, e As EventArgs) Handles Button14.Click
        Letters()
        If A > 25 Then
            A -= 26
        ElseIf A < 0 Then
            A += 26
        End If
        TextBox1.Text += ASC(A)
        TextBox2.Text += ASC(0)
    End Sub

    Private Sub Button15_Click(sender As Object, e As EventArgs) Handles Button15.Click
        Letters()
        If S > 25 Then
            S -= 26
        ElseIf S < 0 Then
            S += 26
        End If
        TextBox1.Text += ASC(S)
        TextBox2.Text += ASC(18)
    End Sub

    Private Sub Button16_Click(sender As Object, e As EventArgs) Handles Button16.Click
        Letters()
        If D > 25 Then
            D -= 26
        ElseIf D < 0 Then
            D += 26
        End If
        TextBox1.Text += ASC(D)
        TextBox2.Text += ASC(3)
    End Sub

    Private Sub Button17_Click(sender As Object, e As EventArgs) Handles Button17.Click
        Letters()
        If F > 25 Then
            F -= 26
        ElseIf F < 0 Then
            F += 26
        End If
        TextBox1.Text += ASC(F)
        TextBox2.Text += ASC(5)
    End Sub

    Private Sub Button18_Click(sender As Object, e As EventArgs) Handles Button18.Click
        Letters()
        If G > 25 Then
            G -= 26
        ElseIf G < 0 Then
            G += 26
        End If
        TextBox1.Text += ASC(G)
        TextBox2.Text += ASC(6)
    End Sub

    Private Sub Button19_Click(sender As Object, e As EventArgs) Handles Button19.Click
        Letters()
        If H > 25 Then
            H -= 26
        ElseIf H < 0 Then
            H += 26
        End If
        TextBox1.Text += ASC(H)
        TextBox2.Text += ASC(7)
    End Sub

    Private Sub Button20_Click(sender As Object, e As EventArgs) Handles Button20.Click
        Letters()
        If J > 25 Then
            J -= 26
        ElseIf J < 0 Then
            J += 26
        End If
        TextBox1.Text += ASC(J)
        TextBox2.Text += ASC(9)
    End Sub

    Private Sub Button21_Click(sender As Object, e As EventArgs) Handles Button21.Click
        Letters()
        If K > 25 Then
            K -= 26
        ElseIf K < 0 Then
            K += 26
        End If
        TextBox1.Text += ASC(K)
        TextBox2.Text += ASC(10)
    End Sub

    Private Sub Button22_Click(sender As Object, e As EventArgs) Handles Button22.Click
        Letters()
        If L > 25 Then
            L -= 26
        ElseIf L < 0 Then
            L += 26
        End If
        TextBox1.Text += ASC(L)
        TextBox2.Text += ASC(11)
    End Sub

    Private Sub Button23_Click(sender As Object, e As EventArgs) Handles Button23.Click
        Letters()
        If Z > 25 Then
            Z -= 26
        ElseIf Z < 0 Then
            Z += 26
        End If
        TextBox1.Text += ASC(Z)
        TextBox2.Text += ASC(25)
    End Sub

    Private Sub Button24_Click(sender As Object, e As EventArgs) Handles Button24.Click
        Letters()
        If X > 25 Then
            X -= 26
        ElseIf X < 0 Then
            X += 26
        End If
        TextBox1.Text += ASC(X)
        TextBox2.Text += ASC(23)
    End Sub

    Private Sub Button25_Click(sender As Object, e As EventArgs) Handles Button25.Click
        Letters()
        If C > 25 Then
            C -= 26
        ElseIf C < 0 Then
            C += 26
        End If
        TextBox1.Text += ASC(C)
        TextBox2.Text += ASC(2)
    End Sub

    Private Sub Button26_Click(sender As Object, e As EventArgs) Handles Button26.Click
        Letters()
        If V > 25 Then
            V -= 26
        ElseIf V < 0 Then
            V += 26
        End If
        TextBox1.Text += ASC(V)
        TextBox2.Text += ASC(21)
    End Sub

    Private Sub RadioButton1_CheckedChanged(sender As Object, e As EventArgs) Handles RadioButton1.CheckedChanged
        Label1.Text = "Cipher Text"
        Label2.Text = "Plain Text"

    End Sub

    Private Sub RadioButton2_CheckedChanged(sender As Object, e As EventArgs) Handles RadioButton2.CheckedChanged
        Label1.Text = "Plain Text"
        Label2.Text = "Cipher Text"
    End Sub

    Private Sub Button3_Click(sender As Object, e As EventArgs) Handles Button3.Click
        Me.Hide()
        Vigenere.Show()
    End Sub

    Private Sub Button27_Click(sender As Object, e As EventArgs) Handles Button27.Click
        Letters()
        If B > 25 Then
            B -= 26
        ElseIf B < 0 Then
            B += 26
        End If
        TextBox1.Text += ASC(B)
        TextBox2.Text += ASC(1)
    End Sub

    Private Sub Button28_Click(sender As Object, e As EventArgs) Handles Button28.Click
        Letters()
        If N > 25 Then
            N -= 26
        ElseIf N < 0 Then
            N += 26
        End If
        TextBox1.Text += ASC(N)
        TextBox2.Text += ASC(13)
    End Sub

    Private Sub Button29_Click(sender As Object, e As EventArgs) Handles Button29.Click
        Letters()
        If M > 25 Then
            M -= 26
        ElseIf M < 0 Then
            M += 26
        End If
        TextBox1.Text += ASC(M)
        TextBox2.Text += ASC(12)
    End Sub

    Private Sub Button30_Click(sender As Object, e As EventArgs) Handles Button30.Click
        TextBox1.Text += " "
        TextBox2.Text += " "
    End Sub

    Private Sub Button31_Click(sender As Object, e As EventArgs) Handles Button31.Click
        TextBox1.Text = ""
        TextBox2.Text = ""
        ii = 0
        Label4.Text = ""
    End Sub
End Class


```
## Vigenère Cipher Form

```vb 
Public Class Vigenere
    Dim ASC = {"A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U", "V", "W", "X", "Y", "Z"}
    Dim vig(100) As Integer
    Dim A As Integer = 0
    Dim B As Integer = 1
    Dim C As Integer = 2
    Dim D As Integer = 3
    Dim E1 As Integer = 4
    Dim F As Integer = 5
    Dim G As Integer = 6
    Dim H As Integer = 7
    Dim I As Integer = 8
    Dim J As Integer = 9
    Dim K As Integer = 10
    Dim L As Integer = 11
    Dim M As Integer = 12
    Dim N As Integer = 13
    Dim O As Integer = 14
    Dim P As Integer = 15
    Dim Q As Integer = 16
    Dim R As Integer = 17
    Dim S As Integer = 18
    Dim T As Integer = 19
    Dim U As Integer = 20
    Dim V As Integer = 21
    Dim W As Integer = 22
    Dim X As Integer = 23
    Dim Y As Integer = 24
    Dim Z As Integer = 25
    Dim ji As Integer = 0
    Dim ii As Integer = 0
    Dim t3 As Integer = 0
    Function Balance()
        If vig(ji) > 25 Then
            While vig(ji) > 25
                vig(ji) -= 26
            End While
        ElseIf vig(ji) < -25 Then
            While vig(ji) > 25
                vig(ji) -= 26
            End While
        End If

    End Function
    Function t3nef()
        If vig(ji) < 0 Then
            vig(ji) += 26
        End If
    End Function
    Private Sub Button4_Click(sender As Object, e As EventArgs) Handles Button4.Click


        If Q > 25 Then
            Q -= 26
        ElseIf Q < 0 Then
            Q += 26
        End If
        If RadioButton1.Checked = True Then

            TextBox1.Text += ASC(Q)
        End If
        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(16)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += Q
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= Q
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += Q
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button5_Click(sender As Object, e As EventArgs) Handles Button5.Click
        If W > 25 Then
            W -= 26
        ElseIf W < 0 Then
            W += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(W)
        End If
        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(22)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += W
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= W
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += W
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button6_Click(sender As Object, e As EventArgs) Handles Button6.Click
        If E1 > 25 Then
            E1 -= 26
        ElseIf E1 < 0 Then
            E1 += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(E1)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(4)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += E1
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= E1
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += E1
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button7_Click(sender As Object, e As EventArgs) Handles Button7.Click

        If R > 25 Then
            R -= 26
        ElseIf R < 0 Then
            R += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(R)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(17)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += R
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= R
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += R
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button8_Click(sender As Object, e As EventArgs) Handles Button8.Click

        If T > 25 Then
            T -= 26
        ElseIf T < 0 Then
            T += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(T)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(19)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += T
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= T
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += T
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button9_Click(sender As Object, e As EventArgs) Handles Button9.Click

        If Y > 25 Then
            Y -= 26
        ElseIf Y < 0 Then
            Y += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(Y)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(24)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += Y
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= Y
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += Y
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button10_Click(sender As Object, e As EventArgs) Handles Button10.Click

        If U > 25 Then
            U -= 26
        ElseIf U < 0 Then
            U += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(U)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(20)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += U
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= U
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += U
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button11_Click(sender As Object, e As EventArgs) Handles Button11.Click

        If I > 25 Then
            I -= 26
        ElseIf I < 0 Then
            I += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(I)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(8)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += I
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= I
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += I
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button12_Click(sender As Object, e As EventArgs) Handles Button12.Click

        If O > 25 Then
            O -= 26
        ElseIf O < 0 Then
            O += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(O)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(14)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += O
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= O
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += O
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button13_Click(sender As Object, e As EventArgs) Handles Button13.Click

        If P > 25 Then
            P -= 26
        ElseIf P < 0 Then
            P += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(P)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(15)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += P
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= P
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += P
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button14_Click(sender As Object, e As EventArgs) Handles Button14.Click

        If A > 25 Then
            A -= 26
        ElseIf A < 0 Then
            A += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(A)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(0)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += A
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= A
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += A
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button15_Click(sender As Object, e As EventArgs) Handles Button15.Click

        If S > 25 Then
            S -= 26
        ElseIf S < 0 Then
            S += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(S)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(18)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += S
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= S
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += S
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button16_Click(sender As Object, e As EventArgs) Handles Button16.Click

        If D > 25 Then
            D -= 26
        ElseIf D < 0 Then
            D += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(D)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(3)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += D
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= D
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += D
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button17_Click(sender As Object, e As EventArgs) Handles Button17.Click

        If F > 25 Then
            F -= 26
        ElseIf F < 0 Then
            F += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(F)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(5)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += F
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= F
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += F
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button18_Click(sender As Object, e As EventArgs) Handles Button18.Click

        If G > 25 Then
            G -= 26
        ElseIf G < 0 Then
            G += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(G)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(6)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += G
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= G
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += G
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button19_Click(sender As Object, e As EventArgs) Handles Button19.Click

        If H > 25 Then
            H -= 26
        ElseIf H < 0 Then
            H += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(H)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(7)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += H
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= H
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += H
        End If
        ji += 1
        ii += 1

    End Sub

    Private Sub Button20_Click(sender As Object, e As EventArgs) Handles Button20.Click

        If J > 25 Then
            J -= 26
        ElseIf J < 0 Then
            J += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(J)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(9)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += J
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= J
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += J
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button21_Click(sender As Object, e As EventArgs) Handles Button21.Click

        If K > 25 Then
            K -= 26
        ElseIf K < 0 Then
            K += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(K)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(10)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += K
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= K
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += K
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button22_Click(sender As Object, e As EventArgs) Handles Button22.Click

        If L > 25 Then
            L -= 26
        ElseIf L < 0 Then
            L += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(L)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(11)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
                vig(ji) += L
            Else
            End If
            If RadioButton4.Checked = True And t3 = 1 Then
                vig(ji) -= L
            End If
            If RadioButton3.Checked = True Then
                vig(ji) += L
            End If
            ji += 1
        ii += 1
    End Sub

    Private Sub Button23_Click(sender As Object, e As EventArgs) Handles Button23.Click

        If Z > 25 Then
            Z -= 26
        ElseIf Z < 0 Then
            Z += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(Z)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(25)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
                vig(ji) += Z
            Else
            End If
            If RadioButton4.Checked = True And t3 = 1 Then
                vig(ji) -= Z
            End If
            If RadioButton3.Checked = True Then
                vig(ji) += Z
            End If
            ji += 1
        ii += 1
    End Sub

    Private Sub Button24_Click(sender As Object, e As EventArgs) Handles Button24.Click

        If X > 25 Then
            X -= 26
        ElseIf X < 0 Then
            X += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(X)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(23)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += X
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= X
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += X
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button25_Click(sender As Object, e As EventArgs) Handles Button25.Click

        If C > 25 Then
            C -= 26
        ElseIf C < 0 Then
            C += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(C)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(2)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += C
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= C
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += C
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button26_Click(sender As Object, e As EventArgs) Handles Button26.Click

        If V > 25 Then
            V -= 26
        ElseIf V < 0 Then
            V += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(V)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(21)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += V
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= V
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += V
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub RadioButton1_CheckedChanged(sender As Object, e As EventArgs) Handles RadioButton1.CheckedChanged
        t3 = 1
        ji = 0
        ii = 0
    End Sub

    Private Sub RadioButton2_CheckedChanged(sender As Object, e As EventArgs) Handles RadioButton2.CheckedChanged
        t3 = 0
        ji = 0
        ii = 0
    End Sub

    Private Sub Button27_Click(sender As Object, e As EventArgs) Handles Button27.Click
        If B > 25 Then
            B -= 26
        ElseIf B < 0 Then
            B += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(B)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(1)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += B
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= B
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += B
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button28_Click(sender As Object, e As EventArgs) Handles Button28.Click

        If N > 25 Then
            N -= 26
        ElseIf N < 0 Then
            N += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(N)
        End If

        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(13)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += N
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= N
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += N
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button29_Click(sender As Object, e As EventArgs) Handles Button29.Click

        If M > 25 Then
            M -= 26
        ElseIf M < 0 Then
            M += 26
        End If
        If RadioButton1.Checked = True Then
            TextBox1.Text += ASC(M)
        End If
        If RadioButton2.Checked = True Then
            TextBox2.Text += ASC(12)
        End If
        If RadioButton2.Checked = True And RadioButton4.Checked = True Then
            vig(ji) += M
        Else
        End If
        If RadioButton4.Checked = True And t3 = 1 Then
            vig(ji) -= M
        End If
        If RadioButton3.Checked = True Then
            vig(ji) += M
        End If
        ji += 1
        ii += 1
    End Sub

    Private Sub Button30_Click(sender As Object, e As EventArgs) Handles Button30.Click
        TextBox1.Text += " "
        TextBox2.Text += " "
    End Sub

    Private Sub Button31_Click(sender As Object, e As EventArgs) Handles Button31.Click
        TextBox1.Text = ""
        TextBox2.Text = ""
        TextBox3.Text = ""
        ji = 0
        ii = 0
    End Sub

    Private Sub Button1_Click(sender As Object, e As EventArgs) Handles Button1.Click

        For ji = 0 To ii - 1
            Balance()
            t3nef()
            TextBox3.Text += ASC(vig(ji))
        Next
        ji += 1
    End Sub

    Private Sub Button2_Click(sender As Object, e As EventArgs) Handles Button2.Click
        Me.Hide()
        Form1.Show()
    End Sub

    Private Sub Button3_Click(sender As Object, e As EventArgs) Handles Button3.Click
        End
    End Sub

    Private Sub RadioButton4_CheckedChanged(sender As Object, e As EventArgs) Handles RadioButton4.CheckedChanged
        Label2.Text = "Cipher Text"
        Label1.Text = "Key"
        RadioButton1.Text = "Key"
        RadioButton2.Text = "Cipher Text"
        Label3.Text = "Message"
    End Sub

    Private Sub RadioButton3_CheckedChanged(sender As Object, e As EventArgs) Handles RadioButton3.CheckedChanged

        Label2.Text = "Message"
        Label1.Text = "Key"
        RadioButton1.Text = "Key"
        RadioButton2.Text = "Message"
        Label3.Text = "Cipher Text"
    End Sub
