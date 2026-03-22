# 🏋️ GymLog — Registro de Treinos

App de registro de treinos estilo Strong/StrongLifts, single-file, sem dependências externas.

## ✅ Funcionalidades

- **Início** — dashboard com próximo treino sugerido, streak, histórico recente
- **Novo Treino** — templates pré-carregados (Upper A/B, Lower A/B) ou treino livre
- **Registro ativo** — cronômetro, log de séries (peso × reps × RPE), timer de descanso automático
- **Histórico** — todos os treinos com volume total, agrupados por mês
- **Detalhe** — visualização e exclusão de treino individual
- **Evolução** — histórico de carga por exercício com PR destacado

## ⚙️ Tecnologia

- HTML + CSS + JavaScript puro — **zero dependências**
- `localStorage` para persistência de dados no navegador
- Single-file (`index.html`) — roda offline

## 🚀 GitHub Pages (hospedagem gratuita)

1. Crie um repositório no GitHub (ex: `gymlog`)
2. Faça upload do `index.html`
3. Vá em **Settings → Pages → Source: main branch / root**
4. Acesse: `https://seu-usuario.github.io/gymlog`

## 📱 Instalar no celular

### iOS (Safari)
Botão compartilhar → **"Adicionar à Tela de Início"**

### Android (Chrome)
Menu (⋮) → **"Adicionar à tela inicial"**

## 💾 Backup dos dados

```js
// Exportar (console do navegador, F12):
console.log(JSON.stringify(JSON.parse(localStorage.getItem('gymlog_v1')), null, 2));

// Importar:
localStorage.setItem('gymlog_v1', JSON.stringify(/* JSON aqui */));
location.reload();
```

## 🔧 Templates

| Template | Ênfase | Exercícios |
|---|---|---|
| Upper A | Tensão Mecânica | Supino, Barra Fixa, Remada Curvada... |
| Lower A | Força | Agachamento, Terra Romeno, Leg Press... |
| Upper B | Volume | Supino Inclinado, Pulldown, Crucifixo... |
| Lower B | Metabólico | Hack Squat, Afundo, Mesa Flexora... |
