# Controle 8.2 – Privileged Access Rights
### ISO/IEC 27001:2022 | Camada 4 · Privilégio · Controle Técnico

🔗 **Deep Dive (interface interativa):** https://gilbertocrv.github.io/identity-management-maturity-iso27001-8-2/

🧭 **Modelo completo de maturidade IAM:** https://gilbertocrv.github.io/iso27001-iam-maturity-model/

---

## Sobre este módulo

Avaliação de maturidade focada no controle de acessos privilegiados — contas administrativas, credenciais de serviço e sessões com poder de alterar o próprio ambiente.

O controle 8.2 representa a transição da camada de governança (5.15–5.18) para a camada de enforcement técnico. Governança sem controle técnico é política sem garantia.

---

## Critérios Avaliados

| Grupo | Foco |
|---|---|
| Concessão e Segregação | Separação de contas administrativas das contas de uso cotidiano |
| PAM e Credenciais | Gestão de senhas privilegiadas via cofre, sem exposição direta |
| Just-in-Time (JIT) | Privilégio temporário, ativado sob demanda e com prazo definido |
| Monitoramento de Sessões | Gravação e logs de todas as ações privilegiadas |

---

## Escala de Maturidade (0–5)

| Nível | Nome | Descrição |
|---|---|---|
| 0 | Inexistente | Senhas administrativas compartilhadas informalmente |
| 1 | Ad-hoc | Cada admin gerencia suas credenciais sem padrão |
| 2 | Documentado | Política definida, mas controle manual |
| 3 | Padronizado | Contas nomeadas e revisões periódicas |
| 4 | Automatizado | PAM com rotação automática de credenciais |
| 5 | Baseado em Risco | JIT, monitoramento contínuo e análise de comportamento |

---

## Funcionalidades do Deep Dive

- Questionário interativo com 12 critérios em 4 grupos
- Score por grupo com barra visual de maturidade
- Cálculo automático a cada seleção
- Exportação em CSV e JSON para evidência e registro
- Exportação em PDF via impressão do navegador

---

## Posição na Arquitetura de Controles

```
Identidade → Autenticação → Autorização → Privilégio
  5.16          5.17 · 8.5     5.15 · 5.18    8.2 · 8.3
```

O 8.2 fecha o ciclo iniciado pela governança: define não apenas quem tem privilégio, mas como esse privilégio é usado, monitorado e revogado.

---

## Sobre o Projeto

Projeto de estudo independente baseado em normas públicas ISO/IEC 27001:2022 e ISO 27701, com aplicação à LGPD.

**Gilberto Gonçalves dos Santos Filho**
Analista de Governança de Identidades — IAM · PAM · GRC
[LinkedIn](https://linkedin.com/in/gilberto-filho-4430a3184) · [GitHub](https://github.com/gilbertocrv)
