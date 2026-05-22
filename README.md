# lab-orq

O objetivo é construir um laboratório de estudo e testes de diversas tecnologias utilizadas em Platform Engineering.
Esse repositório será um centralizador que conecta os outros repositórios relacionado a esse projeto.

Por que dividir por repositórios (Polyrepo + Meta-Orquestrador)?

| Critério | Monorepo Único | Polyrepo + Meta-Orquestrador |
|---|---|---|
| Reutilização | Baixa (acoplado ao lab) | Alta (cada repo pode ser usado em outros projetos) |
| Versionamento | Único para tudo | Independente por domínio (ex: observability v1.2, messaging v0.9) |
| CI/CD | Pesado, executa tudo | Leve, roda apenas o repo alterado |
| Manutenção | Difícil escalar | Escalável, ownership claro |
| Curva de aprendizado | Inicialmente mais fácil | Exige padrão de interface, mas ganha em longo prazo |
