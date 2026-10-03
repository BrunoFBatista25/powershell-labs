***Primeiros passos com o PowerShell***

 ==================================
    *Navegação pelo terminal*
 ==================================

- pwd   [indica a localização]
- ls    [Lista arquivos e pastas do diretório]
    - -Force        [mostra também arquivos ocultos]
    - -Recurse      [lista também o conteúdo das subpastas]
    - -File         [mostra só arquivos]
    - -Directory    [mostra só pastas]
    - -Filter *.txt [filtra por nome ou extensão]
- cd    [Mesma coisa que CMD]
    - -Path         [define a pasta de destino (opcional)]
- cd .. [Mesma coisa que CMD]

 ==================================

       *Arquivos e Pastas*
 ==================================

- mkdir 

    - -Path         [define onde criar a pasta (opcional)]

- New-Item   

    - -ItemType     [File ou Directory: define se cria arquivo ou pasta]
    - -Path / -Name [define o local e o nome]
    - -Value        [cria o arquivo já com conteúdo]
    - -Force        [sobrescreve se já existir]

- Get-Content 

    - -TotalCount 5 [mostra só as 5 primeiras linhas]
    - -Tail 5       [mostra só as 5 últimas linhas]
    - -Wait         [acompanha o arquivo em tempo real, bom para logs]
    - -Raw          [lê tudo como um único texto]

- Remove-Item 
    - -Recurse      [apaga a pasta com tudo dentro]
    - -Force        [apaga arquivos ocultos ou somente leitura]
    - -Confirm      [pergunta antes de apagar]
    - -WhatIf       [simula, mostra o que seria apagado sem apagar]

````shell
mkdir -path Pasta1

cd Pasta1

New-Item test.txt

Get-Content test.txt

Remove-Item test.txt

cd ..

Remove-Item Pasta1
````