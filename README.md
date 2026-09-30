![MyBuy — Amancio.dev](.github/assets/banner.svg)

# MyBuy

**Organizador de compras e orçamento pessoal que funciona no navegador, com dados armazenados no aparelho.**

[Recursos](#recursos) · [Como usar](#como-usar) · [Armazenamento](#armazenamento) · [Estrutura](#estrutura)

## Recursos

| Área | O que você pode fazer |
| --- | --- |
| Orçamento | Definir a renda mensal e acompanhar o saldo restante. |
| Lançamentos | Registrar, editar e consultar receitas e despesas. |
| Organização | Separar compras por categoria, forma de pagamento, apelido de cartão e pessoa. |
| Painel | Consultar os totais de gastos e filtrar o extrato. |
| Backup | Exportar os registros em texto JSON. |

## Como usar

1. Clone ou baixe este repositório.
2. Abra o arquivo `index.html` em um navegador moderno com suporte a IndexedDB.
3. Defina a renda mensal e cadastre seus lançamentos.

Não há instalação de dependências nem etapa de compilação. Também é possível servir a pasta com um servidor estático local.

## Armazenamento

O aplicativo utiliza **IndexedDB** para guardar os registros no navegador. Os dados não são sincronizados automaticamente entre dispositivos. Limpar os dados do navegador pode apagar os lançamentos; a opção **Exportar backup (JSON)** permite guardar uma cópia.

A identificação de cartões usa somente apelidos. O aplicativo não precisa do número, da validade, da senha ou do CVV.

## Estrutura

```text
MyBuy/
├── index.html   # Interface, estilos e lógica do aplicativo
└── README.md    # Apresentação e instruções de uso
```

**Tecnologias:** HTML, CSS, JavaScript e IndexedDB.
