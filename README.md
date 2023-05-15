
# k6




![Logo](https://images.g2crowd.com/uploads/product/image/social_landscape/social_landscape_9fcecb565c7303e367747d46e315effe/k6.png)


## Referência

 - [Documentação do K6](https://k6.io/docs/)

 ## Pré-requisitos para começar a usar o k6:

 - Conhecimento intermediário de programação, especialmente em Javascript;
 - Conhecimento intermediário do protocolo HTTP ;
 - Conhecimento intermediário de API;
 - Conhecimento básico de CLI;


## Instalação

Faça a instação do pacote K6 gratuitamente em [k6.io](https://k6.io/docs/get-started/installation/) seguindo o sistema operacional que você possui. Para Windows faça uso do gerenciador de pacotes [ Chocolatey ](https://chocolatey.org/)

```bash
  choco install k6

```
    
# Documentação

Esses códigos são scripts de teste de carga **escrito em JavaScript** usando a biblioteca K6. O objetivo aqui é aprender sobre o K6 e como realizar scripts de teste de carga.
## K6

O K6 é uma ferramenta de código aberto de teste de carga e desempenho desenvolvida em Go que permite simular uma grande quantidade de usuários virtuais (VUs) interagindo com um sistema em um determinado período de tempo. Ele pode ser executado localmente em um ambiente de desenvolvimento ou em um ambiente de nuvem.
## Usando k6

- **Thresholds**: Thresholds são condições de limite definidas pelo usuário que devem ser atendidas para que um teste de carga seja considerado bem-sucedido. 
- **VUs**: VUs (Usuários Virtuais) são os usuários simulados que interagem com o sistema durante um teste de carga.
- **Duration**: A duração do teste de carga é o período de tempo durante o qual o teste é executado. Ele pode ser definido em segundos, minutos, horas ou dias, dependendo dos requisitos do teste
- **Checks**: É usada para verificar se a resposta de uma solicitação HTTP satisfaz um ou mais critérios.

## Estágios do ciclo de vida do teste

```javascript
	// 1. Inicialização

	export function setup() {
	  // 2. Configuração
	}

	export default function (data) {
	  // 3. Execução
	}

	export function teardown(data) {
	  // 4. desmontagem
	}
}
```

## Usando k6-reporter
- Adicione a linha de código na seção de Inicialização para importar o reporter do K6, é uso no exemplo **registro-usuario-relatorio.js**

```bash
  import { htmlReport } from "https://raw.githubusercontent.com/benc-uk/k6-reporter/main/dist/bundle.js";

```



## Aprendizado

K6 é uma ferramenta poderosa para testes de carga e estresse de aplicações. Com ela, é possível criar simulações realistas para avaliar o desempenho de sistemas. Aprendendo os conceitos básicos e a sintaxe, é possível criar scripts eficientes e obter insights valiosos sobre o comportamento da sua aplicação sob carga. Com K6, pode descobrir gargalos e otimizar a performance da sua aplicação antes mesmo de colocá-la em produção.
