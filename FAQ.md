# FAQ – Controle 8.2: Privileged Access Rights

Perguntas frequentes sobre o módulo de maturidade em gestão de acessos privilegiados.

---

## Sobre o Controle

**O que é o controle 8.2 da ISO 27001:2022?**
Define os requisitos para gestão de acessos privilegiados — contas com poder de alterar configurações, permissões e o próprio ambiente. Vai além da autorização comum (5.18) ao exigir controles técnicos sobre como o privilégio é concedido, usado e monitorado.

**Qual a diferença entre 5.18 e 8.2?**
O 5.18 governa quem pode acessar o quê — é o processo de concessão e revisão de permissões. O 8.2 trata especificamente de acessos com poder elevado: administradores, DBAs, contas de serviço. A lógica é: 5.18 define a regra, 8.2 garante o enforcement técnico nos casos de maior risco.

**O que são contas privilegiadas?**
São contas com capacidade de alterar o ambiente além do uso comum: contas de administrador local, Domain Admin, root, DBA, contas de serviço e contas de emergência (break-glass). Diferem das contas comuns pelo impacto potencial de uso indevido.

---

## Sobre os Conceitos

**O que é PAM (Privileged Access Management)?**
Conjunto de processos e ferramentas para controlar o acesso de contas privilegiadas. Na prática, inclui cofre de credenciais (as senhas ficam armazenadas e rotacionadas automaticamente, sem que o usuário as conheça), controle de sessões e gravação de atividades.

**O que é Just-in-Time (JIT)?**
Modelo de concessão de privilégio temporário: o acesso elevado é ativado apenas quando necessário, com prazo definido, e revogado automaticamente ao fim da atividade. Reduz drasticamente a janela de exposição comparado ao modelo de privilégio permanente.

**O que são contas zumbi?**
Contas com privilégios elevados que permanecem ativas sem uso — geralmente criadas para uma atividade específica e nunca desativadas. São um dos principais vetores de risco em ambientes sem revisão periódica de acessos privilegiados.

**Por que contas genéricas (admin, root) são um problema?**
Porque eliminam a rastreabilidade individual. Se dez pessoas usam a mesma conta "admin", é impossível determinar quem executou uma ação específica em caso de incidente ou auditoria.

---

## Sobre o Formulário

**Como interpretar o score por grupo?**
Cada grupo representa uma dimensão do controle 8.2. Scores baixos em grupos específicos indicam onde concentrar esforços de melhoria — por exemplo, score 1.5 em JIT sugere que a organização ainda usa privilégios permanentes.

**O que exportar: CSV ou JSON?**
CSV é mais adequado para registrar evidências em planilhas ou sistemas de GRC. JSON é indicado para integração com ferramentas ou para preservar o histórico estruturado da avaliação ao longo do tempo.

**O formulário é uma ferramenta de auditoria formal?**
Não. É uma ferramenta educacional para reflexão e diagnóstico. Os resultados não substituem uma auditoria formal baseada em evidências, mas podem orientar a priorização de controles e servir como ponto de partida para conversas com gestores e auditores.

**Com que frequência devo reavaliar?**
A cada ciclo de revisão de acessos privilegiados — recomendado trimestralmente para ambientes com alta criticidade, ou semestralmente como mínimo.

---

## Sobre o Projeto

**Este projeto segue alguma norma específica?**
Sim. A base normativa é a ISO/IEC 27001:2022, com referências à ISO 27701 quando o controle toca dados pessoais, e à LGPD no contexto brasileiro. O projeto não cobre ISO 31000 (gestão de riscos) ou outros frameworks como COBIT e PCI-DSS intencionalmente — o escopo é deliberadamente focado.

**Posso usar este material em projetos profissionais?**
Sim. O conteúdo é baseado em normas públicas e foi desenvolvido de forma independente. Adapte conforme a realidade da organização onde for aplicar.

**Onde estão os outros controles da série?**
No modelo completo: https://gilbertocrv.github.io/iso27001-iam-maturity-model/
