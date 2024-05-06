# Unity-2DPlayerControl-Script

⭐使用建議:

將player sprite與capsule collider分成兩個物件，組成群組，並將此程式套用於capsule collider上。程式的Animator及Player則參考player sprite之Animator及sprite

此程式支援多項animator parameters，以便操控player sprite之animation

*提供之parameters*

float speed:橫軸速度

float vertical_speed:縱軸速度

bool climbing:是否黏在牆上

bool jumping:是否正在跳躍

trigger attacking:是否按下左鍵



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

Coyote_time:離開地面後的Coyote_time秒(使用Time.deltaTime)內，允許跳躍

Jump_spare:若在落地前的Jump_spare秒(使用Time.deltaTime)內按下跳躍，允許跳躍

Walljump_strength:踢強跳時，RigidBody.velocity設為(±Walljump_strength,walljump_strength)
