# Radar de Leads
## Problema
Descobrir empresas de diferentes segmentos e organizar a prospecção sem perder o histórico dos contatos.

## Evolução e minha participação
Após a primeira versão, realizei testes de funcionamento e testes manuais de API com Postman. A experiência de uso orientou melhorias no painel e no fluxo de prospecção. O projeto evoluiu também com DuckDB e Overture Maps para ampliar a descoberta por nicho e localização.

## Implementação
- Node.js, TypeScript e Express na API.
- SQLite para persistência operacional.
- DuckDB como motor de consulta a arquivos Parquet da Overture Maps.
- Filtros por localização, categorias e termos de pesquisa.
- Carteira de leads e acompanhamento de contatos, oportunidades, tarefas e propostas.
- Validação de entradas e tratamento de indisponibilidade, limites e falhas das fontes.

DuckDB e SQLite têm papéis distintos: o primeiro consulta a fonte de descoberta; o segundo mantém os dados operacionais da aplicação.

## Um exemplo de melhoria
O fluxo de contato permite confirmar uma abordagem manual, persistir o evento e avançar para a próxima empresa. Os contatos continuam disponíveis no filtro correspondente após recarregar ou reiniciar a aplicação.

## Validação
Além dos meus testes manuais com Postman, o histórico de desenvolvimento registra validações de persistência, recuperação de rascunhos após falhas e uma etapa com 71 testes automatizados aprovados. Esse número se refere àquela etapa de validação, não a uma execução contínua publicada neste repositório.

## Aprendizados
- Transformar dificuldades observadas no uso em requisitos concretos.
- Distinguir coleta de dados, persistência e apresentação.
- Testar a API e os fluxos completos da interface.
- Tratar falhas de rede e de gravação com feedback ao usuário.
- Usar IA como apoio ao desenvolvimento e participar da validação e das decisões do produto.

Este é um estudo de caso. Não contém a base de contatos, credenciais ou código operacional do sistema.

[Voltar ao perfil](../README.md)
