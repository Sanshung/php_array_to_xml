# php array to xml
PHP array to xml. Конвертирует array в xml фаил

$xml = new ArrayToXML();
$arr['title'] = 'Sanshung';
$arr['link'] = array('@rel'=> 'self', '@href'=> 'http://site.com');

$xmlResult = $xml->buildXML($arr, 'feed', array('xmlns'=> 'http://www.w3.org/2005/Atom', 'xmlns:g' => 'http://base.google.com/ns/1.0'));

header('Content-Type: text/xml; charset-utf-8');
echo $xmlResult;

return return.xml

