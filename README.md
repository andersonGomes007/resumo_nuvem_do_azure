# Desvendando os Serviços de Nuvem do Azure

## Resumo do Lab: Criando Máquinas Virtuais na Azure

Neste laboratório, aprendemos como criar uma máquina virtual no portal da Azure, explorando as opções de disponibilidade e tipos de armazenamento, que influenciam diretamente no custo mensal.

---

## Níveis de SLA (Service Level Agreement)

Os SLAs representam o compromisso da Microsoft com a disponibilidade dos serviços. Quanto maior o número de "noves" no SLA, menor será o tempo de inatividade permitido.

| SLA        | Tempo de Inatividade por Semana | Por Mês           | Por Ano            |
|------------|-------------------------------|-------------------|--------------------|
| **99%**    | 2h 8min                        | 7,2 horas         | 3,65 dias          |
| **99,9%**  | 10 minutos                     | 43,2 minutos      | 8,76 horas         |
| **99,95%** | 5 minutos                      | 21,6 minutos      | 4,38 horas         |
| **99,99%** | 1 minuto                       | 4,32 minutos      | 52,56 minutos      |
| **99,999%**| 6 segundos                     | 25,9 segundos     | 5,26 minutos       |

### Observações:
- Quanto mais "9" o SLA tiver, **menor será o tempo de indisponibilidade** permitido.
- SLAs mais altos são ideais para aplicações críticas, onde a interrupção do serviço deve ser mínima.

---

## Considerações ao Criar uma Máquina Virtual no Azure

- O **portal da Azure** permite configurar opções de **alta disponibilidade**, como:
  - **Conjuntos de disponibilidade (Availability Sets)**
  - **Zonas de disponibilidade (Availability Zones)**

- A **escolha do tipo de armazenamento** (HDD, SSD Standard ou SSD Premium) afeta:
  - O **desempenho** da máquina virtual
  - O **custo mensal** total do serviço

---

## Conclusão

Ao criar uma VM na Azure, é essencial considerar:
- O nível de SLA desejado para o seu serviço
- A estratégia de disponibilidade
- O tipo de armazenamento adequado ao seu orçamento e necessidades de desempenho

Essas escolhas impactam diretamente na **resiliência** da aplicação e no **custo final**.
