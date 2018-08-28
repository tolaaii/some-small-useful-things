# _Một vài ứng dụng của tôi..._
## Hẹn giờ tắt máy
* #### Ảnh chụp màn hình

![UI](https://raw.githubusercontent.com/tolaaii/some-small-useful-things/hen_gio_tat_may/Untitled.png)

* #### Mã nguồn mở

```csharp
private void timer1_Tick(object sender, EventArgs e)
{
    if (isStop == false) // Bắt đầu đếm ngược
    {
        if (timeLeft <= 10)
        {
            notifyIcon1.BalloonTipText = "Còn " + timeLeft + " giây trước khi tắt máy !";
            if (isShow == true) notifyIcon1.ShowBalloonTip(1000);
        }
        if (timeLeft > 0)
        {
            label6.Text = tools1.secToClock(timeLeft);
            notifyIcon1.Text = "Time remaining: " + tools1.secToClock(timeLeft);
            timeLeft -= 1;
        }
        else
        {
            timer1.Stop();
            // Tắt máy
            System.Diagnostics.Process.Start("shutdown", "/s /hybrid /f /t 0");
        }
    }
}
```

* #### Tải về: [Link 1](https://github.com/tolaaii/some-small-useful-things/blob/master/hen_gio_tat_may/hen_gio_tat_may_v100.rar) hoặc                      [Link 2](https://drive.google.com/open?id=1ao36kSTJcYF8S_dL_rvwDMIAvh41Zcuo)  


## Dọn dẹp thư mục Download


## Taskkill
