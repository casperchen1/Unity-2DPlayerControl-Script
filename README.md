# Unity-2DPlayerControl-Script
*以下為參數說明:*
Acceleration:加速Vector的SmoothDamp之deltatime值(1/Acceleration)
Acclination:減速Vector的SmoothDamp之deltatime值(1/Acclination)
Max_speed:速度Vector之絕對值上限
Angle:角色移動時的傾斜角度
Jump_height:跳躍時RigidBody.velocity.y(以下簡稱y速度)的值
Jump_thershold:當y速度的值>Jump_thershold時放開跳躍鍵，可以中斷跳躍
Falling_speed:掉落速度上限(輸入正值)
Falling_plunge:中斷跳躍時，立即將y速度設為-1*Falling_plunge
Falling_acceleration:掉落時的RigidBody.gravityscale
Coyote_time:離開地面後的Coyote_time秒(Time.deltaTime)內，允許跳躍
Jump_spare:若在落地前的Jump_spare秒(Time.deltaTime)內按下跳躍，允許跳躍
Walljump_strength:踢強跳時，速度設為(±Walljump_strength,walljump_strength)
