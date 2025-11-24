# Análise de Problemas de IHC - LATAM Airlines Brasil

## 📋 Sobre o Projeto

Este projeto apresenta uma análise crítica de **5 problemas reais de Interação Humano-Computador (IHC)** identificados no website oficial da **LATAM Airlines Brasil** (latamairlines.com/br/pt), fundamentada nas **10 Heurísticas de Usabilidade de Jakob Nielsen (1994)**.

A análise foi realizada através de inspeção heurística do website real, capturando elementos de HTML e identificando violações das heurísticas de usabilidade.

## 🎯 Problemas Identificados

### 1. Modal de Login Intrusivo Bloqueando Conteúdo
**Heurística #3: Controle e Liberdade do Usuário**

Modal de login aparece automaticamente na página inicial, bloqueando o acesso ao conteúdo e forçando o usuário a tomar uma ação antes de explorar o site.

### 2. Formulário de Busca sem Feedback Visual de Foco
**Heurística #1: Visibilidade do Status do Sistema**

Campos de origem e destino no formulário de busca não mostram claramente qual campo está ativo/focado, causando confusão ao digitar.

### 3. Terminologia Técnica no Programa LATAM Pass
**Heurística #2: Correspondência entre o Sistema e o Mundo Real**

Programa de fidelidade usa termos como 'acumular milhas', 'resgatar', 'categoria', 'upgrade de cabine' sem explicações claras para usuários iniciantes.

### 4. Ofertas de Voos sem Informações Completas de Preço
**Heurística #5: Prevenção de Erros**

Ofertas mostram apenas preço base sem indicar se inclui taxas, bagagem ou outras cobranças adicionais, levando a surpresas desagradáveis no checkout.

### 5. Excesso de Tabs e Opções sem Hierarquia Clara
**Heurística #8: Estética e Design Minimalista**

Formulário principal tem 8 tabs (Voos, Pacotes, Hospedagem, Carros, Seguros, Upgrade, eSIM, Universal) criando sobrecarga cognitiva e dificultando foco na tarefa principal.

## 🚀 Como Executar

### Pré-requisitos

- Node.js 18+ instalado
- pnpm instalado globalmente

### Instalação e Execução

```bash
# 1. Instalar pnpm globalmente (se ainda não tiver)
npm install -g pnpm

# 2. Instalar dependências do projeto
pnpm install

# 3. Iniciar servidor de desenvolvimento
pnpm dev
```

O projeto estará disponível em: **http://localhost:3001**

### Build de Produção

```bash
# Gerar build otimizado
pnpm build

# Visualizar build localmente
pnpm preview
```

## 📁 Estrutura do Projeto

```
ihc_projeto_final/
├── client/
│   ├── src/
│   │   ├── components/
│   │   │   ├── mockups/          # Mockups visuais dos problemas
│   │   │   │   ├── ModalLoginMockup.tsx
│   │   │   │   ├── FormularioFeedbackMockup.tsx
│   │   │   │   ├── LatamPassMockup.tsx
│   │   │   │   ├── OfertasPrecoMockup.tsx
│   │   │   │   └── NavegacaoTabsMockup.tsx
│   │   │   └── Header.tsx         # Componente de cabeçalho
│   │   ├── data/
│   │   │   └── problems.ts        # Dados dos 5 problemas
│   │   ├── pages/
│   │   │   ├── Home.tsx           # Página inicial (lista)
│   │   │   ├── ProblemDetail.tsx  # Página de detalhes
│   │   │   └── Comparison.tsx     # Página de comparação
│   │   ├── App.tsx                # Rotas principais
│   │   └── main.tsx               # Entry point
│   └── index.html
├── package.json
├── vite.config.ts
├── tailwind.config.ts
├── tsconfig.json
├── todo.md                        # Checklist de features
├── ANALISE_LATAM.md              # Análise do website LATAM
└── README.md                      # Este arquivo
```

## 🎨 Tecnologias Utilizadas

- **React 19** - Framework UI
- **TypeScript** - Tipagem estática
- **Vite** - Build tool e dev server
- **Tailwind CSS 4** - Estilização
- **shadcn/ui** - Componentes UI
- **Wouter** - Roteamento
- **Lucide React** - Ícones

## 📚 Metodologia

A análise foi conduzida seguindo os seguintes passos:

1. **Captura de HTML Real**: Acesso ao website oficial da LATAM Airlines Brasil (latamairlines.com/br/pt) e captura de elementos reais da interface
2. **Inspeção Heurística**: Identificação de violações das 10 Heurísticas de Usabilidade de Nielsen (1994)
3. **Documentação**: Registro detalhado de cada problema com:
   - Descrição técnica
   - Impacto no usuário real (histórias contextualizadas)
   - Fundamentação teórica
   - Proposta de redesign
   - Contexto real da LATAM
4. **Prototipação**: Criação de mockups visuais mostrando problema e solução lado a lado

## 🌟 Funcionalidades

- ✅ **Página Inicial**: Lista organizada dos 5 problemas com descrições curtas
- ✅ **Página de Detalhes**: Análise completa de cada problema com mockup visual
- ✅ **Página de Comparação**: Visualização lado a lado (ANTES/DEPOIS) com tabs
- ✅ **Mockups Realistas**: Componentes baseados no HTML real da LATAM
- ✅ **Navegação Intuitiva**: Header com links para todas as seções
- ✅ **Design Responsivo**: Funciona em desktop, tablet e mobile
- ✅ **Contexto Brasileiro**: Exemplos com cidades brasileiras, preços em R$, programa LATAM Pass

## 📖 Referências

- Nielsen, J. (1994). **10 Usability Heuristics for User Interface Design**. Nielsen Norman Group.
- Website oficial da LATAM Airlines Brasil: [latamairlines.com/br/pt](https://www.latamairlines.com/br/pt)

## 👨‍💻 Autor

Projeto desenvolvido como trabalho final de Interação Humano-Computador (IHC).

## 📝 Licença

Este projeto é para fins educacionais e acadêmicos.

---

**Nota**: Este projeto é uma análise crítica independente e não possui afiliação oficial com a LATAM Airlines.
