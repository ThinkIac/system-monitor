# system-monitor

Mini painel de uso de CPU, memória, armazenamento e rede.

Repositório: https://github.com/ThinkIac/system-monitor.

## Uso no ThinkIac

Este pacote foi extraído de `packages/system-monitor`. Preserve a identidade `system-monitor` do manifest ao instalá-lo em um workspace Lógos. Views, rotas, ferramentas e hooks são descobertos pelo runtime e dependem dos provedores correspondentes. Esta extração publica o código atual; não converte JavaScript para LógosType nem implementa instalação por perfil.

## Dependências e validação

Consulte `package.json` e os imports para as capacidades exigidas do host.

O pacote não declara scripts npm de build/teste. Os testes existentes acompanham o fonte; a composição completa requer o host ThinkIac.

## Segurança e dados locais

Credenciais devem ser configuradas no ambiente de destino. Não acompanham esta extração bancos, sessões, uploads, perfis pessoais, arquivos `.env`, caches ou backups. As exclusões foram registradas em relatório externo à publicação. Configure segredos pelo host, sem incluí-los em commits.


## Registros encontrados no código

- `router`: `stats`.
- `tool`: `getSystemStats`.

A lista é um inventário estático e pode incluir registros em testes; não garante disponibilidade sem os provedores do host.

Há imports relativos para diretórios superiores. A instalação isolada e a composição por perfil precisam resolver esses vínculos antes de remover a cópia da base.

