# _Một vài ứng dụng của tôi..._
## Hẹn giờ tắt máy
* #### Ảnh chụp màn hình
![UI](https://tolaaii.github.io/some-small-useful-things/images/hen_gio_tat_may_UI.png)
* #### Mã nguồn mở

```csharp
private void timer1_Tick(object sender, EventArgs e)
{
    if (isStop == false) // Đếm ngược
    {
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
* #### Tải về: [Link 1](https://github.com/tolaaii/some-small-useful-things/blob/master/hen_gio_tat_may/hen_gio_tat_may_v102.rar) hoặc                      [Link 2](https://drive.google.com/open?id=1cCNuQZjLx7ElcbyococxZD_qGQR-veKk)  
* #### Changelog: [Xem](https://tolaaii.github.io/some-small-useful-things/docs/hengiotatmay-changelog.html)


## Dọn dẹp thư mục Download
* #### Ảnh chụp màn hình
![UI](https://tolaaii.github.io/some-small-useful-things/images/clean_UI.png)
* #### Tải về
* #### Changelog: [Xem](https://tolaaii.github.io/some-small-useful-things/docs/cleaner-changelog.html)

## Taskkill
