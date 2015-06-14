Resumo de Compiladores
======================

## Representação Intermediária do Código
	- Facilita alguma tarefa do compilador
	- Serve para análise do programa (Checagem de tipos ou otimização)
	- Control-flow graph (Descreve o fluxo do programa)
	- Points-to graph (Mapa que associa endereços possíveis de referenciamento)
	- Call graph (Identifica o chamador e o chamado)

## Análise Estática
	- Técnica para extrair informação de um software em tempo de compilação
	- Conceito Fundamental: Dependência de Código
	- Dataflow Analysis: Determina o comportamento dinâmico de um programa olhando apenas o código estático (Por exemplo, quanto registradores serão necessários para a execução do programa?)
	- Liveness Analysis (Não vi no slide do professor)
	- Slicing de programas: Técnica de compreensão de codigo, muito utilizada para depuração.
			- Slicing estático: 
				1. Descobre dependência em tempo de compilação
				2. Impreciso
			- Slicing dinâmico:
				1. Descobre dependências em tempo de execução
				2. Subgrafo do grafo estático de dependendências
				3. Leva em consideração a função main
			- Quizz Time: Slicing Estático é melhor que Slicing Dinâmico?

