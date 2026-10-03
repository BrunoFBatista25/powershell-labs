
***Primeiros passos com o PowerShell***

 ==================================
    *Navegação pelo terminal*
 ==================================

- pwd   [indica a localização]
- ls    [Lista arquivos e pastas do diretório]
- cd    [Mesma coisa que CMD]
- cd .. [Mesma coisa que CMD]

 ==================================

       *Arquivos e Pastas*
 ==================================

- mkdir       [Mesmo coisa que CMD]
- New-Item    [cria arquivo]
- Get-Content [mostra/lê o Contéudo do arquivo]
- Remove-Item [Apaga a o Arquivo ou pasta inteira]

````shell
mkdir Pasta1

cd Pasta1

New-Item test.txt

Get-Content test.txt

Remove-Item test.txt

Remove-Item Pasta1

````
