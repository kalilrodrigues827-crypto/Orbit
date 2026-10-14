# Orbit 0.2 — Alpha local

Evolução do protótipo 0.1. Interface futurista responsiva, múltiplos servidores e canais independentes, criação de servidores/canais, envio, edição e exclusão de mensagens, busca por canal, edição de apelido e persistência no localStorage.

## Executar

Requer Node.js 20+.

```bash
npm install
npm run dev
```

Abra o endereço mostrado pelo Vite. Para gerar uma versão web estática: `npm run build`.

## Limitações importantes

Este projeto ainda é **um protótipo local**. O armazenamento local não sincroniza dispositivos, não é uma base segura de produção e pode ser apagado ao limpar dados do navegador. A sala de voz é apenas uma simulação de interface, sem áudio real. Não existem cadastro, backend, criptografia de ponta a ponta, notificações push nem clientes nativos nesta versão. A próxima etapa é um backend com autenticação, autorização, PostgreSQL e WebSockets; depois voz/vídeo com WebRTC/SFU e clientes multiplataforma.

## Estrutura

- `src.jsx`: estado da interface, canais, mensagens e persistência local
- `style.css`: design responsivo
- `index.html`: ponto de entrada

## Segurança para a próxima etapa

Implementar autenticação e sessões, checagem de permissão no servidor, validação de entradas, rate limiting, política de retenção, relatórios de abuso, testes e observabilidade antes de permitir usuários reais.
