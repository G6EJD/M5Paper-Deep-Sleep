# M5Paper-Deep-Sleep
  digitalWrite(GPIO_NUM_5, LOW);
  gpio_hold_en(GPIO_NUM_2);
  gpio_hold_en(GPIO_NUM_5);
  esp_sleep_enable_timer_wakeup(((1 * 60) - 10) * 1000000LL); // -10 secs to account for internal delays
  esp_deep_sleep_start();
