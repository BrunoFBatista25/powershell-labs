# ⚡ PowerShell Labs

Laboratório de estudo de escrita em **PowerShell**: scripts, exercícios e experimentos para praticar automação no Windows e aprofundar a rotina de suporte técnico N1.

![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)

---

## 🎯 Objetivo

Praticar a escrita de scripts PowerShell de forma progressiva, partindo dos fundamentos até automações úteis no dia a dia de **Service Desk** e **infraestrutura de TI**, como diagnóstico de rede, coleta de informações do sistema e tarefas repetitivas.

---

## 🗂️ Estrutura do repositório

```
powershell-labs/
├── Notes/       # anotações de estudo (conceitos, comandos, boas práticas)
├── Pratica/     # scripts e exercícios práticos (.ps1)
├── LICENSE      # licença MIT
└── README.md
```

| Pasta | Conteúdo |
| ----- | -------- |
| 📝 **Notes** | Anotações organizadas por tema, com explicações e exemplos de comandos |
| 🧪 **Pratica** | Scripts `.ps1` escritos para fixar o que foi estudado nas notas |

---

## ▶️ Como executar

1. Clone o repositório:
```powershell
   git clone https://github.com/BrunoFBatista25/powershell-labs.git
   cd powershell-labs
```

2. Se necessário, libere a execução de scripts na sessão atual:
```powershell
   Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```

3. Execute um script da pasta `Pratica`:
```powershell
   .\Pratica\nome-do-script.ps1
```

> ⚠️ Leia o código antes de rodar qualquer script, principalmente em máquinas de produção.

---

## 🧪 Exemplo

```powershell
# Testa a conectividade com um host e mostra o resultado
$destino = "8.8.8.8"

if (Test-Connection -ComputerName $destino -Count 2 -Quiet) {
    Write-Host "✅ $destino respondeu." -ForegroundColor Green
} else {
    Write-Host "❌ Sem resposta de $destino." -ForegroundColor Red
}
```

---

## 🛠️ Tecnologias

| Ferramenta | Uso |
| ---------- | --- |
| PowerShell 5.1 / 7+ | Escrita e execução dos scripts |
| Windows | Ambiente de testes |
| Git e GitHub | Versionamento |

---

## 🗺️ Roadmap de estudo

- [ ] Fundamentos da linguagem
- [ ] Funções e parâmetros
- [ ] Tratamento de erros (`try/catch`)
- [ ] Manipulação de arquivos e logs
- [ ] Scripts de diagnóstico de rede
- [ ] Automação de rotinas de suporte N1

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 👤 Autor

**Bruno Felipe**, Analista de Suporte N1 | Redes, Windows, Linux e PowerShell

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/brunofelipedorsbatista)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/BrunoFBatista25)

---

*"Entender o problema real, não só o sintoma."*
