# 🇦🇴 Gestor Financeiro KD (Kwanza Digital)

Um sistema simples e eficiente para controlo de dívidas e créditos, desenvolvido especialmente para o contexto angolano. Esta aplicação permite gerir quem nos deve e a quem devemos, com suporte para pagamentos parciais e relatórios mensais.

## 🚀 Funcionalidades

* **Registo de Fluxo:** Escolha entre "Eu Devo" (Débito) ou "Devem-me" (Crédito).
* **Gestão de Amortizações:** Permite fazer pagamentos parciais (parcelas) ou totais.
* **Cálculo Automático:** O sistema abate o valor pago e mantém o saldo restante atualizado.
* **Relatórios Flexíveis:** Filtre por mês e ano ou visualize o histórico completo de todos os meses.
* **Persistência de Dados:** Os dados são guardados no `LocalStorage` do navegador, não sendo perdidos ao fechar a página.
* **Design Responsivo:** Adaptado para utilização em computadores, tablets e telemóveis.

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Estrutura semântica dos formulários e tabelas.
* **CSS3:** Estilização moderna, uso de variáveis (`:root`), Grid e Flexbox para responsividade.
* **JavaScript (Vanilla):** Lógica de cálculos, manipulação do DOM e gestão de armazenamento local.

## 📂 Estrutura de Dados

Cada registo na aplicação segue este modelo de objeto:

```javascript
{
    id: 1710435600000,      // Identificador único (Timestamp)
    tipo: "devo",           // "devo" ou "receber"
    pessoa: "Maninho",      // Nome do contacto
    valor: 50000,           // Valor original da dívida
    restante: 30000,        // Quanto ainda falta pagar
    data: "2026-03-14",     // Data de origem ou liquidação
    motivo: "Empréstimo",   // Descrição da operação
    concluido: false,       // Estado da dívida
    isParcela: false        // Define se o registo é uma amortização parcial
}
