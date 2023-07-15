# Dígito verificador, modulo 11, nosso numero sicredi em php -
/*
sicredi_11($bit, $nosso_numero, $cedente, $posto, $agencia){
$nosso_numero=str_pad($nosso_numero,5,"0",STR_PAD_LEFT);
$ano=date('y');
$numero=$agencia[0]*4;
$numero+=$agencia[1]*3;
$numero+=$agencia[2]*2;
$numero+=$agencia[3]*9;
$numero+=$posto[0]*8;
$numero+=$posto[1]*7;
$numero+=$cedente[0]*6;
$numero+=$cedente[1]*5;
$numero+=$cedente[2]*4;
$numero+=$cedente[3]*3;
$numero+=$cedente[4]*2;
$numero+=$ano[0]*9;
$numero+=$ano[1]*8;
$numero+=$bit*7;
$numero+=$nosso_numero[0]*6;
$numero+=$nosso_numero[1]*5;
$numero+=$nosso_numero[2]*4;
$numero+=$nosso_numero[3]*3;
$numero+=$nosso_numero[4]*2;
$divisao = floor($numero / 11);
$mutiplicacao = 11 * $divisao;
$resto = $numero - $mutiplicacao;

$dv = 11 - $resto;
if($dv == 11){
	$dv ='0';
}
}
if($dv == 10){
$dv ='0';
}
return $dv;
*/
