<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Me dar um beijin?</title>
</head>
<body>
    <div class="box">
        <p>Me dar um beijin?</p>
        <div class="button-container">
            <button>
                <a id="yes">Sim</a>
            </button>
            <button id="no">Não</button>
        </div>
    </div>
    
    <script>
        let button = document.getElementById('no')
        let height = window.innerHeight-50
        let width = window.innerWidth-50

        button.addEventListener('mouseover', function(){
            button.style.position='absolute'
            button.style.top=Math.random()*height+'px'
            button.style.left=Math.random()*width+'px'
        })

        const btn = document.getElementById('yes')
        btn.addEventListener('click', function(){
            alert('Obrigado, voce clicou!')
        })
    </script>
</body>
</html>
