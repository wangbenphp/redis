#使用方法

require_once 'RedisHandle.php';

//Redis配置文件
$config = ['host' => '127.0.0.1', 'port' => '6379', 'auth' => '', 'database' => 0];
$redis = RedisHandle::getInstance($config);

$res = $redis->keys('*');

echo '<pre>';
print_r($res);