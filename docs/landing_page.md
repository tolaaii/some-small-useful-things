#   Một vài ứng dụng của tôi...
## Hẹn giờ tắt máy
#### Ảnh chụp màn hình

![UI](https://github.com/tolaaii/some-small-useful-things/blob/master/hen_gio_tat_may/Untitled.png)

#### Mã nguồn mở

~~~~
private void timer1_Tick(object sender, EventArgs e)
        {
            if(isStop == false)
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
                    ////// begin shutdown
                    System.Diagnostics.Process.Start("shutdown", "/s /hybrid /f /t 0");
                }
            }
        }
~~~~

#### Tải về: [Link](https://github.com/tolaaii/some-small-useful-things/blob/master/hen_gio_tat_may/hen_gio_tat_may_v100.rar)  
## Dọn dẹp thư mục Download


## Taskkill
