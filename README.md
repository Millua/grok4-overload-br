# Grok-4 Resiste a Overload Semântico em PT-BR: Benchmark com 6 LLMs

**Autor:** Smile Luã S Gonçalves 
**Local:** Jequié, BA, Brasil  
**Email:** smile14lua@gmail.com  
**Data:** 27/10/2025  

---

## Resumo
Testei **6 LLMs + Grok-4** com uma charada cheia de números (overload semântico).  
**Grok-4 responde em ~350 tokens.**  
Outros modelos gastam **400–800+ tokens** tentando calcular ruído.

---

## Prompt completo
> [quiz.txt](quiz.txt) *(1500 km, 35 pedágios, Fibonacci, etc.)*

---

## Resultados

| Modelo | Latência | Tokens | Ruído ignorado? |
|--------------------|------------------|--------|-----------------|
| **Grok-4** | **Imediato** | ~350 | SIM |
| Perplexity AI | 1 parágrafo | ~450 | SIM |
| Gemini 2.5 Pro | 1 linha | ~400 | SIM |
| Meta AI (Llama 4) | 2 parágrafos | ~700 | NÃO |
| ChatGPT (GPT-4o) | 3 parágrafos | ~650 | NÃO |
| DeepSeek V3.2 | Explicação longa | ~800+ | NÃO |

---

## Evidência
- [screenshots/](screenshots/) → 6 capturas (incl. Grok-4 self-test)  
- [quiz.txt](quiz.txt) → prompt exato  

---

## Reprodução
1. Cole o conteúdo de `quiz.txt` em cada modelo  
2. Meça o tempo até **"VOCÊ"**  
3. **Grok-4 vence em foco e velocidade**

---

> **Grok-4 me ajudou na análise técnica, contagem de tokens e redação (uso 100% ético).**

**Disponível para entrevista remota (GMT-3).**  
Interessado em **bug bounty ou contrato**.

---

**Repo:** https://github.com/Millua/grok4-overload-br
