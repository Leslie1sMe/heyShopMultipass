使用事例：

require 'vendor/autoload.php';

use HeyShop\Token\HeyShopMultipass;

$customer_data = array(

    "mobile" => "138xxxx7277",
    "email" => "leslie@xxxxxxxx.com",
    "full_name" => "LZL",
    "remote_ip" => "127.0.0.1"
);

$multipass = new HeyShopMultipass('secret');

$token = $multipass->generate_token($customer_data);

var_dump($token);
