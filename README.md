# WhatsApp-API-PHP-SDK
Lightweight PHP library for WhatsApp API to send the whatsappp messages in PHP provided by [online-live-support.com](https://online-live-support.com)

online-live-support.com WhatsApp API PHP SDK

#Example usage

```<?php
$curl = curl_init();
curl_setopt_array($curl, array(
  CURLOPT_URL => 'https://v2.onlinelivesupport.com/chats/sendMessageText?id={{id}}',
  CURLOPT_RETURNTRANSFER => true,
  CURLOPT_ENCODING => '',
  CURLOPT_MAXREDIRS => 10,
  CURLOPT_TIMEOUT => 0,
  CURLOPT_FOLLOWLOCATION => true,
  CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
  CURLOPT_CUSTOMREQUEST => 'POST',
  CURLOPT_POSTFIELDS =>'{
    "message":"hello",
    "jid":"receivernumber"
}',
));
$response = curl_exec($curl);
curl_close($curl);
echo $response;
```
[Start Free Trial Now
](https://online-live-support.com)

**NOTE**: you need replace id (session id) which you have recieved it via Email and WhatsApp during subscription started with Online Live Support. If you have lost it, please email us at info@online-live-support.com
