# Desafio DevSecOps — Gerenciador de Tarefas

## Sobre o Projeto
Este repositório faz parte do desafio prático do módulo de DevSecOps da ADA Tech.
Você receberá este projeto com vulnerabilidades propositais e uma pipeline incompleta.
Seu objetivo é **implementar a pipeline de segurança** e **corrigir as vulnerabilidades**.

## Estado atual
A pipeline está **incompleta**. Os steps de segurança precisam ser implementados por você.

## Sua missão
1. Implementar os steps de segurança no `pipeline.yml`
2. Fazer a pipeline **quebrar** ao detectar os problemas
3. Corrigir as vulnerabilidades encontradas
4. Fazer a pipeline **passar** com tudo verde ✅
5. Documentar o funcionamento da pipeline neste README

## O que implementar
- [ ] Secrets Scanning com **Gitleaks**
- [ ] SAST com **Semgrep**
- [ ] SCA com **Grype**
- [ ] Assinatura do artefato com cosign
- [ ] Deploy com **GitHub Pages**

## Como a pipeline funciona
Desafio DevSecOps - Gerenciador de Tarefas
Este repositório faz parte do desafio prático de DevSecOps da ADA Tech. O objetivo do projeto foi implementar uma esteira de CI/CD automatizada com foco em segurança, aplicando a regra de break the build (o deploy só acontece se os portões de segurança passarem).
URL de Produção
A aplicação em produção pode ser acessada em:
https://julianadagnone.github.io/projeto-devsecop-desafio/
Portões de Segurança da Pipeline
A pipeline roda automaticamente a cada envio de código (push) e possui 3 verificações principais:
1.	Secrets Scanning (Gitleaks)
o	O que faz: Analisa o código e o histórico do repositório em busca de senhas, chaves de API ou segredos expostos.
o	Importância: Evita o vazamento acidental de credenciais sensíveis no código.
2.	SAST - Static Application Security Testing (Semgrep)
o	O que faz: Analisa o código-fonte em busca de más práticas de programação e falhas de segurança (como o uso inseguro de eval e problemas de innerHTML que podem gerar XSS).
o	Importância: Permite encontrar e corrigir vulnerabilidades no próprio código antes de ir para produção.
3.	SCA - Software Composition Analysis (Grype)
o	O que faz: Verifica as dependências de terceiros no arquivo package.json em busca de vulnerabilidades conhecidas.
o	Importância: Garante que bibliotecas desatualizadas ou vulneráveis sejam corrigidas via atualização de versão.


## URL de Produção
https://julianadagnone.github.io/projeto-devsecop-desafio/
