# Relatório de Laboratório: Ataque de Força Bruta com Medusa

Este repositório documenta a simulação de ataques de força bruta contra serviços de rede utilizando a ferramenta Medusa no Kali Linux, mapeando vulnerabilidades em protocolos comuns.

## 🛠️ Configuração do Ambiente
- **Sistema Operacional Atacante:** Kali Linux (Bare Metal)
- **Ferramenta de Ataque:** Medusa v2.3

## 📌 Testes Executados e Evidências

### 1. Ataque de Força Bruta contra FTP (Porta 21)
Ataque simulado contra o serviço de transferência de arquivos.
- **Resultado:** Credenciais encontradas com sucesso (`msfadmin / msfadmin`).

### 2. Ataque de Força Bruta contra SMB (Porta 445)
Ataque direcionado ao protocolo de compartilhamento de arquivos.
- **Resultado:** Credenciais válidas obtidas (`msfadmin / msfadmin`).

### 3. Ataque contra Formulário Web (DVWA)
Simulação de quebra de autenticação em uma aplicação web integrada.
- **Resultado:** Acesso administrativo comprometido (`admin / password`).

## 🛡️ Medidas de Mitigação Propostas

1. **Políticas de Bloqueio de Conta:** Bloquear temporariamente contas após 3 a 5 tentativas falhas consecutivas.
2. **Implementação de CAPTCHA e 2FA:** Adicionar validações de segundo fator e desafios visuais para mitigar requisições automatizadas.
3. **Complexidade de Senhas:** Exigir senhas robustas que resistam a ataques baseados em dicionários comuns (*wordlists*).
