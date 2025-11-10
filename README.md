# HC Sprint 4 - Front-End (React + Vite + TypeScript)

**Projeto:** Sistema de Gestão (Sprint 4)  
**Equipe:**  
- Bruno Martins Bettio (RM564939)  
- Otávio Ferreira Barreto Santos (RM565960)  
- Raphael Salomão Chamma (RM564765)  
- Samuel Tenório Caval (RM565881)

- Link repositório:https://github.com/TaikaWaititi/hc-1tdsa-front-sprint.git
- Link Vercel: https://hc-1tdsa-front-sprint-git-main-bruno-martins-projects-0f5b7137.vercel.app

## Visão geral
Este projeto é a evolução da Sprint 3, adaptada para **React + Vite + TypeScript** conforme as exigências da Sprint 4 do Challenge 2025.  
Inclui integração com a API pública **ViaCEP** para consulta de endereços por CEP.

## Principais adições nesta entrega
- Componente integrado na **Home** para buscar endereço por CEP (`SearchCepForm`).
- Hook reutilizável `useCepSearch` para consumo da API ViaCEP.
- Componentes `CepResult` e `LoadingSpinner`.
- Tipagem TypeScript para resposta da ViaCEP (`src/types/viaCep.ts`).
- Estilização com **TailwindCSS** (utilitários personalizados para as cores do projeto).
- README com instruções para execução e deploy.

## Tecnologias
- React 18
- Vite
- TypeScript
- TailwindCSS
- API externa: https://viacep.com.br/

## Observações sobre o componente de CEP
- O campo de CEP aceita somente números. Deve ter 8 dígitos para realizar a consulta.
- Tratamento de erros implementado (CEP inválido, não encontrado, erros de rede).
- A integração consome `https://viacep.com.br/ws/{cep}/json/`.

