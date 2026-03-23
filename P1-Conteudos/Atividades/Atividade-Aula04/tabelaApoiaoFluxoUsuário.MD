------------------------------
	##Folha de Apoio – Construção de Fluxo de Usuário
Persona escolhida: Ricardo, o Gestor de Frota (42 anos).
Objetivo da Persona: Garantir a disponibilidade da frota e prever manutenções sem depender de GPS.
------------------------------
Etapas do Fluxo

| Etapa | Descrição da Ação do Usuário | Sistema/Aplicativo responde | Sentimento esperado |
|---|---|---|---|
| Início | Abre o app no pátio para atualizar o odômetro do veículo. | Exibe dashboard com resumo da frota e botão de input rápido. | Vigilância (Focado em não esquecer o dado). |
| Etapa 1 | Digita a quilometragem (KM) atual do caminhão ABC-123. | Valida o KM e calcula a distância para a próxima revisão. | Controle (Sentindo que o sistema está atualizado). |
| Etapa 2 | Recebe um alerta de que a troca de óleo deve ocorrer em 500km. | Altera o status do veículo para "Laranja" e sugere agendamento. | Urgência/Cálculo (Avaliando quando parar o carro). |
| Etapa 3 | Clica em "Agendar" e anexa foto do orçamento da oficina. | Registra a intenção de manutenção e salva o documento. | Alívio (Planejamento concluído). |
| Fim | Confirma a realização do serviço após o retorno do veículo. | Reseta o contador de manutenção e volta o status para "Verde". | Dever Cumprido (Ativo protegido). |

------------------------------
Decisões

| Decisão | Condição | Caminho A | Caminho B |
|---|---|---|---|
| Validação de KM | O KM inserido é menor que o anterior? | Erro: Pede para conferir o odômetro. | Sucesso: Segue para o cálculo de revisão. |
| Status do Alerta | KM está a <10% da revisão? | Alerta: Exibe aviso de manutenção imediata. | Silencioso: Apenas atualiza o banco de dados. |
| Urgência Operacional | Precisa do carro para hoje? | Adiar: Posterga o alerta por +200km (com justificativa). | Parar: Inicia o processo de check-out para oficina. |

------------------------------
Oportunidades de Melhoria

| Etapa ou decisão | Possível ponto de dor | Oportunidade de melhoria |
|---|---|---|
| Entrada de Dados | Erro de digitação manual do KM. | Implementar leitura de odômetro via OCR (foto do painel). |
| Geração de Alerta | Alerta ignorado por ser apenas visual. | Enviar notificação push/WhatsApp automática para o Ricardo. |
| Inatividade | Ficar dias sem atualizar o KM. | Cálculo Preditivo: Sistema estima o KM com base na média histórica. |

------------------------------
