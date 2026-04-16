Sistema de Automação Comercial Omnichannel (IA + Low-Code)

O Problema: Microempreendedores enfrentam dificuldades na gestão de pedidos, atendimento 24h e organização de entregas por falta de ferramentas acessíveis ou conhecimento em gestão.

A Solução: Desenvolvi um ecossistema inteligente utilizando n8n como orquestrador, integrando a Evolution API para comunicação em tempo real. O sistema utiliza Inteligência Artificial (LLMs) para um atendimento humanizado, PostgreSQL para persistência de dados e Google Sheets como interface de gestão simplificada para o usuário final.

Funcionalidades:

Atendimento e vendas automatizadas 24/7.

Gestão de agendamentos e horários de funcionamento dinâmicos.

Triagem de pedidos e integração com logística de entrega.

Scripting personalizado em JavaScript para tratamento de dados complexos.
Upgrade de Estabilidade e Controle de Fluxo (n8n + Evolution API)

Implementação de Filtro de Caducidade: Adicionado nó de código JavaScript para ignorar mensagens recebidas há mais de 60 segundos (evitando disparos em massa após reinicialização do sistema).

Lógica Anti-Loop (Self-Reply): Filtragem de mensagens enviadas pela própria instância (fromMe: true) para evitar loops infinitos de IA.

Redundância de LLM: Migração temporária do Mistral para Groq para contornar erros de Rate Limit (429) e garantir baixa latência.
