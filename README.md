# Gerenciamento de Atendimentos

Este é um projeto simples de gerenciamento de atendimentos, onde você pode registrar atendimentos e fazer o acompanhamento de registros. O sistema permite adicionar atendimentos e registros, calcular a porcentagem de registros em relação aos atendimentos, e armazenar dados diários e mensais.

## Funcionalidades

- **Contagem de Atendimentos e Registros**: Permite adicionar atendimentos e registros, com a atualização automática da porcentagem de registros.
- **Cálculo de Porcentagem**: Exibe a porcentagem de registros em relação aos atendimentos realizados.
- **Histórico Diário**: Armazena os dados dos atendimentos e registros do dia, incluindo a porcentagem calculada.
- **Histórico Mensal**: Exibe o total de atendimentos e registros do mês, com a porcentagem mensal calculada.
- **Limpar Histórico**: Permite limpar os históricos diários e mensais.
- **Tema Escuro**: O projeto utiliza um tema escuro para uma interface mais agradável em ambientes de pouca luz.

## Como Usar

1. Abra o arquivo `index.html` no seu navegador.
2. Insira os atendimentos e registros clicando nos botões `+1 Atendimento` e `+1 Registro`.
3. A porcentagem será automaticamente calculada e exibida na interface.
4. Clique em `Armazenar Dados do Dia` para salvar o histórico diário.
5. Os dados mensais são atualizados automaticamente com base nos dados do dia.
6. Para limpar o histórico, utilize o botão `Limpar Tudo`.

## Funcionalidades Adicionais

### Armazenamento Local

Os dados do histórico são armazenados localmente no navegador, o que significa que as informações serão preservadas mesmo após a atualização da página.

### Histórico de Atendimentos

- **Histórico Diário**: Exibe os atendimentos e registros do dia, junto com a porcentagem.
- **Histórico Mensal**: Exibe o total de atendimentos e registros no mês, com a porcentagem mensal.

## Tecnologias Utilizadas

- **HTML**: Para a estrutura da página.
- **CSS**: Para o estilo e tema escuro.
- **JavaScript**: Para a lógica de contagem, cálculo de porcentagem e armazenamento de dados localmente.

## Exemplo de Uso

```html
<div class="container">
    <h1>Gerenciamento de Atendimentos</h1>
    <input type="number" id="atendimentos" value="0" />
    <button onclick="adicionarAtendimento()">+1 Atendimento</button>
    <input type="number" id="registros" value="0" />
    <button onclick="adicionarRegistro()">+1 Registro</button>
    <p>Porcentagem: <span id="porcentagem">0%</span></p>
</div>
