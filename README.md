# Language

Translate the site into your language
https://poeditor.com/join/project/4zQZx6tHPM

PHP

function Language ($lang)
{
	$url = 'https://raw.githubusercontent.com/MinterCat/Language/master/MinterCat_'.$lang.'.json';
	$data = file_get_contents($url);
    $jsonCalled = json_decode($data);
    return $jsonCalled;
}

$lang = 'Russian';
$language = Language($lang);
$language->Play;
