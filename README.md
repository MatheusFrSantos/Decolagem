# Sistema de Verificação para Decolagem de Missão

## Descrição do Projeto
Este projeto tem como objetivo simular um sistema de verificação de telemetria de uma missão espacial, determinando se a nave está apta para decolagem.

A partir da leitura de dados como temperatura, energia e pressão, o sistema realiza verificações com base em limites seguros e retorna uma decisão final:

- ✅ PRONTO PARA DECOLAR  
- ❌ DECOLAGEM ABORTADA  

---

## Funcionalidades

- Leitura de dados de entrada
- Verificação de condições críticas
- Tomada de decisão automatizada
- Cálculo de autonomia energética

## Dados analisados

O sistema considera os seguintes parâmetros:

- Temperatura interna
- Temperatura externa
- Integridade estrutural (0 ou 1)
- Nível de energia (%)
- Pressão dos tanques
- Status dos módulos críticos (0 ou 1)

## Lógica de decisão

A decolagem só é autorizada se **todas as condições estiverem dentro dos limites seguros**. Caso contrário, a decolagem é abortada.

Exemplo de regras:
- Energia mínima: 80%
- Integridade estrutural: 1 (OK)
- Temperaturas dentro da faixa segura
- Pressão adequada
- Módulos ativos 1 (OK)

## Análise Energética

O sistema calcula a autonomia com base em:

- Capacidade total (kWh)
- Carga atual (%)
- Consumo estimado
- Perdas energéticas

Fórmula utilizada:

- Energia disponível = capacidade * (carga/100) 
- Energia real = energia disponível - perdas 
- Autonomia = energia real/consumo

## Como executar

1. Acesse o notebook (.ipynb)
2. Execute as células
3. Insira os valores solicitados
4. Observe o resultado final no console

## Prints da execução

<img width="1222" height="945" alt="Lançamento positivo" src="https://github.com/user-attachments/assets/1fb4a404-f516-47fd-84a2-5f408cf3a7cb" />
<img width="1222" height="972" alt="Lançamento negativo" src="https://github.com/user-attachments/assets/d30d6840-9615-4075-b28d-3c144148591c" />
<img width="1190" height="466" alt="Energia" src="https://github.com/user-attachments/assets/f1557b9a-7c60-4c8f-a932-fdd79fb698f5" />
## Repositório no GitHub:

https://github.com/MatheusFrSantos/Decolagem.git

## 👨‍💻 Autor
Matheus Freitas da Silva Santos

Projeto desenvolvido como parte da atividade integradora.
