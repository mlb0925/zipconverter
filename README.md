# 安装方法
```
composer require mlb0925/zipconverter
```
# 使用方法
```
$zip = new \Mlb0925\zipConverter();
$zip->setRecursiveness(true); //default is false
$zip->addFolder(
    array(
        './', //path of the current file
        'F:\wamp2\www\yml', //Windows Path
        '/var/www/html'  //linux path
    )
);
$zip->setZipPath('./files.zip'); //Set your Zip Path with your Zip File's Name
$result = $zip->createArchive();

echo "<pre>";var_dump($result);echo "</pre>";
```
