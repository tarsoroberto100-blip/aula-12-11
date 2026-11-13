# Registro do experimento com IA — Grupo [N]

**Tema:** tema-5: teste de softwares com IA 
**Integrantes:** [Tarso, Tiago, Jefferson, pedro Eduardo]  
**IA usada:** ChatGPT 
**Data:** 12/11/2026

---

## 1. Pesquisa

**Respostas às perguntas-guia do cartão:**

1. **O que fazem as ferramentas?**  
   A **mabl** automatiza testes funcionais de aplicações e usa recursos de IA para ajudar a criar, executar e manter testes. A **Applitools Eyes** compara a aparência das telas com imagens de referência para encontrar alterações visuais inesperadas. A **testRigor** permite escrever cenários de teste em linguagem natural e automatizar ações sem depender tanto de scripts tradicionais.

2. **Que problemas de teste de software elas resolvem?**  
   A mabl procura reduzir o trabalho repetitivo e a manutenção de testes que deixam de localizar elementos após mudanças na interface. A Applitools ajuda a encontrar defeitos visuais — como desalinhamentos, elementos ausentes e mudanças inesperadas de layout — que podem passar despercebidos em testes funcionais. A testRigor reduz a barreira técnica para criar testes automatizados e ajuda a diminuir a dependência de seletores frágeis e código escrito manualmente.

3. **Quais são as limitações?**  
   Nenhuma das três garante que um software esteja livre de erros. A mabl não consegue recuperar todos os testes automaticamente: por exemplo, a documentação informa que etapas com seletores CSS ou XPath personalizados não recebem auto-healing e que o auto-healing avançado é limitado a execuções na nuvem. A Applitools exige revisão das diferenças e manutenção das imagens de referência; conteúdo dinâmico pode exigir configurações especiais. A testRigor depende de instruções e validações bem definidas; seu plano gratuito torna públicos os testes e resultados, e algumas capacidades dependem dos planos pagos.

**Fontes consultadas** (nome do site e link):

- **mabl Help — How auto-heal works:** https://help.mabl.com/hc/en-us/articles/19078583792404-How-auto-heal-works
- **mabl Help — Test execution overview:** https://help.mabl.com/hc/en-us/articles/17780538073108-Test-execution-overview
- **mabl — Pricing:** https://www.mabl.com/pricing
- **Applitools — Documentação:** https://applitools.com/docs/
- **Applitools Help — Dynamic content:** https://help.applitools.com/hc/en-us/articles/360006915412-Dynamic-content
- **G2 — Avaliações de usuários da Applitools:** https://www.g2.com/products/applitools/reviews
- **testRigor — Documentação de linguagem:** https://testrigor.com/docs/language
- **testRigor — Planos e cadastro:** https://testrigor.com/sign-up/
- **testRigor — FAQ:** https://testrigor.com/faq/

---

## 2. Experimento

As três tentativas abaixo registram os três pedidos feitos durante a conversa para aprofundar a pesquisa, um para cada ferramenta.

### Tentativa 1

**Prompt enviado:**

```text
Explique o que faz a ferramenta [mabl], qual problema de teste de software
ela resolve e quais são as limitações dela. Cite as fontes.
```

**Resumo da resposta da IA** (trecho mais importante):

```text
A mabl é uma plataforma que utiliza inteligência artificial para automatizar testes de software. Ela permite criar, executar e analisar testes de aplicações web, dispositivos móveis e APIs. Seu recurso Auto-healing tenta localizar novamente elementos da interface quando eles sofrem alterações.

O problema principal que procura resolver é a manutenção trabalhosa dos testes automatizados. Porém, o auto-healing não é infalível, e a ferramenta não substitui profissionais de QA nem garante que todas as regras de negócio estejam corretas.
```

**Aproveitamos:** a explicação do objetivo da mabl e do auto-healing, pois a documentação oficial confirma que a ferramenta tenta adaptar etapas gravadas quando elementos mudam.

**Corrigimos ou descartamos:** não tratamos o auto-healing como uma correção garantida. A documentação informa que seletores CSS/XPath personalizados não recebem esse recurso e que o auto-healing avançado é exclusivo das execuções na nuvem.

### Tentativa 2

**O que mudamos no prompt e por quê:** mantivemos a mesma estrutura, mas trocamos a ferramenta para investigar uma solução especializada em testes visuais e comparar suas funções com as de automação funcional.

**Prompt enviado:**

```text
Explique o que faz a ferramenta [Applitools], qual problema de teste de software
ela resolve e quais são as limitações dela. Cite as fontes.
```

**Resumo da resposta:**

```text
A Applitools Eyes utiliza inteligência artificial e visão computacional para comparar capturas de tela com imagens de referência e identificar diferenças visuais inesperadas, como mudanças de layout, textos desalinhados e elementos que desapareceram.

Ela ajuda a encontrar defeitos visuais que testes funcionais tradicionais podem não perceber. Entretanto, as diferenças precisam ser analisadas e as imagens de referência atualizadas quando uma mudança é intencional. Conteúdo dinâmico também pode exigir configurações específicas.
```

**Aproveitamos:** a distinção entre teste visual e teste funcional, além da explicação sobre imagens de referência (baselines) e conteúdo dinâmico.

**Corrigimos ou descartamos:** não generalizamos a função do Applitools Eyes para todos os produtos da empresa. A documentação atual apresenta também a plataforma Applitools com recursos de testes funcionais, visuais e de API; a descrição de comparação visual refere-se principalmente ao Eyes.

### Tentativa 3

**O que mudamos no prompt e por quê:** substituímos a ferramenta por uma solução que permite escrever testes em linguagem natural, para investigar se ela reduz a necessidade de programação e quais restrições permanecem.

**Prompt enviado:**

```text
Explique o que faz a ferramenta [testRigor], qual problema de teste de software
ela resolve e quais são as limitações dela. Cite as fontes.
```

**Resumo da resposta:**

```text
A testRigor permite criar e executar testes automatizados usando instruções em linguagem natural. O usuário pode descrever ações, como abrir a página de login, preencher e-mail e senha e verificar uma mensagem.

Ela procura reduzir a dependência de programação e de seletores técnicos. Ainda assim, depende de instruções e validações corretas. O plano gratuito é público, ou seja, os testes e resultados podem ser vistos por outras pessoas.
```

**Aproveitamos:** o exemplo de instrução em linguagem natural e a observação sobre a privacidade do plano gratuito, confirmada pela página oficial de cadastro.

**Corrigimos ou descartamos:** não afirmamos que a ferramenta elimina completamente a programação ou a necessidade de conhecimento técnico. Também registramos que recursos e plataformas disponíveis variam conforme o plano; por exemplo, testes de aplicações desktop nativas do Windows são indicados como recurso pago na página oficial.

---

## 3. Onde a IA errou

| Erro da IA | Como descobrimos (requisito, código, conta ou fonte) | O certo é |
| --- | --- | --- |
| A resposta sobre a Applitools apresentou a ferramenta como se fosse somente visual. | A documentação atual da Applitools diferencia o produto Eyes, voltado a testes visuais, da plataforma mais ampla, que também anuncia testes funcionais e de API. | Explicar que o Applitools Eyes é focado em testes visuais, mas a plataforma Applitools possui outros recursos. |
| A explicação do auto-healing da mabl poderia dar a impressão de que ele funciona em qualquer situação. | A documentação oficial lista exceções: etapas com seletores CSS/XPath personalizados não recebem auto-healing; o avançado funciona em execuções na nuvem. | O auto-healing ajuda a recuperar alguns testes, mas tem condições e limites técnicos. |
| A descrição do plano gratuito da testRigor poderia levar a pensar que todos os recursos são gratuitos e privados. | A página oficial de cadastro informa que o plano gratuito é público e que testes e resultados ficam visíveis; também diferencia os planos privados e empresariais. | O plano gratuito existe, mas é público e tem limitações; recursos privados e adicionais dependem de planos pagos. |
| Preços e condições comerciais podem ficar desatualizados. | As páginas oficiais de preços e cadastro podem ser atualizadas e variam conforme plano, uso e negociação. | Consultar a página oficial no momento da contratação; não tratar valores mencionados anteriormente como permanentes. |

---

## 4. Recomendação do grupo

**Use IA para:**

- Ajudar a pesquisar ferramentas e resumir documentação técnica.
- Sugerir cenários de teste e exemplos de casos de uso.
- Comparar funcionalidades e identificar possíveis limitações.
- Ajudar a escrever testes iniciais e organizar resultados.

**Não confie na IA para:**

- Garantir que um sistema não tenha bugs.
- Decidir sozinha se uma mudança é um defeito ou uma alteração intencional.
- Validar regras de negócio sem critérios claros.
- Confirmar preços, planos ou limitações sem consultar a documentação atualizada.
- Aprovar uma versão do software sem revisão humana.

**A melhor dica de prompt que aprendemos:**

Peça sempre três coisas separadas: o que a ferramenta faz, qual problema de teste resolve e quais limitações possui. Solicite fontes oficiais e, quando possível, avaliações de usuários. Depois, confira se cada afirmação realmente aparece nas fontes e diferencie a promessa do fabricante da experiência relatada por usuários.
