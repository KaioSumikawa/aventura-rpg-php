<?php
// Variáveis iniciais do jogo
$nomeJogo = "Aventura PHP";
$nomeJogador = "Fabiano";

// Mensagem de boas-vindas
echo "<h1>Bem-vindo, $nomeJogador, ao Mundo dos Games!</h1>";
echo "<p>Iniciando nossa jornada<br> na Lógica de Programação em PHP</p>";
echo "<h2>Jogo: $nomeJogo</h2><hr>";

// Características do personagem
$nomePersonagem = "FabianoFake";
$nivel = 1;
$classe = "Mago";
$vidaMaxima = 100;
$vidaAtual = 100;
$manaMaxima = 50;
$manaAtual = 50;
$forca = 8;
$inteligencia = 15;
$destreza = 12;

// Atributos derivados
$poderAtaque = $forca * 2;
$poderMagico = $inteligencia * 3;
$velocidade = $destreza * 1.5;

// Exibição da ficha técnica
echo "<h1>Ficha Técnica do Personagem</h1>
    <div style='border:1px solid #ccc; padding: 15px; width: 300px; font-family: Arial;'>
        <h2>$nomePersonagem</h2>
        <p><strong>Classe:</strong> $classe</p>
        <p><strong>Nível:</strong> $nivel</p>
        <p><strong>Vida:</strong> $vidaAtual / $vidaMaxima</p>
        <p><strong>Mana:</strong> $manaAtual / $manaMaxima</p>
        <hr>
        <p><strong>Força:</strong> $forca</p>
        <p><strong>Inteligência:</strong> $inteligencia</p>
        <p><strong>Destreza:</strong> $destreza</p>
        <hr>
        <p><strong>Poder de Ataque:</strong> $poderAtaque</p>
        <p><strong>Poder Mágico:</strong> $poderMagico</p>
        <p><strong>Velocidade:</strong> $velocidade</p>
    </div>";

// Simulação de combate
$danoCausado = $poderMagico;
$vidaInimigo = 100;
$vidaInimigoRestante = $vidaInimigo - $danoCausado;

echo "<h2>Resultado de Combate</h2>
    <p>$nomePersonagem lançou um feitiço e causou <strong>$danoCausado</strong> de dano!</p>
    <p>Vida restante do inimigo: <strong>$vidaInimigoRestante</strong> / $vidaInimigo</p>";
?>
