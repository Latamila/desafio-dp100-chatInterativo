# desafio-dp100-chatInterativo
Desenvolva um chat interativo onde seja possível realizar perguntas e obter respostas contextuais fundamentadas nos arquivos.


Crie um arquivo chamado readme.md , deixe alguns prints descreva o processo, alguns insights e possibilidades que você aprendeu durante o conteúdo após a IA analisar suas sentenças

<h2> PLAYGROUND CRIADO </h2>
![image](https://github.com/user-attachments/assets/32e63ab8-538d-407e-9c3c-a350c3d09afb)

<h2> IMPLANTANDO UM MODELO GPT 4o  * COLOQUE EXATAMENTE A REGIÃO SWEDEN CENTRAL OU OUTRA QUE SUA PLATAFORMA RECOMENDAR </h2>

Disse isso já no título porque lá no final, não consigo implantar o modelo como um aplicativo web porque esse serviço não está disponível na região que escolhi, mas depois eu refiz o projeto e deu certinho, só não mudei as imagens daqui para efeito de portifólio, estas já são de efeito satisfatório. Depois, logo incluirei as imagens do aplicativo web implementado dado que é um serviço que não fica disponível que se implanta. 

Se você está fazendo o Bootcamp da DIO saiba que o projeto não pede implantação, mas para o seu dia a dia profissional podemos ir alem do esperado!

![image](https://github.com/user-attachments/assets/2ceba7fb-6980-4593-95af-f2869393cf2f)

Implantar o modelo básico. 

Selecione o GPT-4.o

![image](https://github.com/user-attachments/assets/19bcd339-db11-4f8a-8ca3-3dcd5bd4e4d4)

![image](https://github.com/user-attachments/assets/0a59f043-214c-43ae-ab1d-0dd5b939bb41)

<h2> Vamos criar um outro modelo com modelo text-embeddings-3-large </h2>

![image](https://github.com/user-attachments/assets/dd19ab4e-aecf-459e-9556-8967cbdc112a)

![image](https://github.com/user-attachments/assets/18cfe594-3286-474a-abeb-b20b8a6f6049)

O modelo GPT-4o vai conversar em linguagem natural e outro modelo vai passar meu texto para vetores. 

<h1> PREPARANDO O AMBIENTE </h1>

![image](https://github.com/user-attachments/assets/efb49498-6e83-4787-b4f7-4f70afc20701)

Altere o comportamento do CHATBOT na lacuna e clique em APLICAR ALTERAÇÕES

![image](https://github.com/user-attachments/assets/3057a1d6-35c7-4ec8-86c3-17f232bc5c23)

Clique em Adicionar Dados, logo abaixo dos comandos anteriores.

![image](https://github.com/user-attachments/assets/97e14a68-82e5-440f-948e-e1309256b6bd)


![image](https://github.com/user-attachments/assets/db3367f4-da87-4a57-9a9d-fe8bee2c3edb)

![image](https://github.com/user-attachments/assets/13d9ea05-9c81-430d-9e20-c0159e7c53a9)

![image](https://github.com/user-attachments/assets/9b78ec1b-4d17-426f-9eb0-158f1c4bacfe)

![image](https://github.com/user-attachments/assets/d7fc5fb0-a3a0-4684-8c7b-8f2cd5fc9e9b)

![image](https://github.com/user-attachments/assets/a1f22bae-96a9-4dbc-ab8f-6e083889980c)

Como vimos na imagem acima, houve uma mensagem reclamando sobre a obrigatoriedade de se criar um AI SEARCH. 
Volte no PORTAL AZURE, no mesmo GRUPO DE RECURSOS, criar um recurso e busque por AZURE AI SEARCH. 

![image](https://github.com/user-attachments/assets/db49920d-bc74-44ca-8cbe-f9005375007e)

Altere o tipo de preço. Eu escolhi o gratuito. 


![image](https://github.com/user-attachments/assets/e548e6f1-f4ed-4d9a-b6ee-2423029e6723)

![image](https://github.com/user-attachments/assets/7de3ead0-c2ae-4212-9db5-f0269aaf79fc)

![image](https://github.com/user-attachments/assets/251e0827-72e8-44e8-a72e-1014e0aecec3)

Se caso, você for escolher o BÁSICO, não esqueça de excluir o laboratório ao terminar para não gerar mais custos. 
Pode pedir para Examinar e Criar.

Cl![image](https://github.com/user-attachments/assets/510915cf-5bf6-438d-80df-7a57001779c4)

IR PARA O RECURSO 

![image](https://github.com/user-attachments/assets/6467df94-0b08-4edf-ac2b-543addf5362f)

Retorne ao AI FOUNDRY e clique em AVANÇAR. 


![image](https://github.com/user-attachments/assets/9ad43595-252d-4cfb-a01d-b1798a058e99)

CLIQUE EM CONECTAR O RECURSO DE AI SEARCH
![image](https://github.com/user-attachments/assets/011a8252-1973-4920-babb-78534d221cb8)

CLIQUE EM ADICIONAR CONEXÃO

![image](https://github.com/user-attachments/assets/4c051415-1cbe-4063-97b2-5f0b4774c6ee)

CLIQUE E SELECIONE O SEU AI SEARCH 

![image](https://github.com/user-attachments/assets/0b704d41-fddd-473f-8cb7-db7b8d2fe744)

CLIQUE EM AVANÇAR


![image](https://github.com/user-attachments/assets/c6f44d3b-47b5-460c-ac77-489704c75deb)

Escolha o modelo de Embeddings que você anteriormente criou em um dos modelos, no caso o text-embeddings-3-large

EXAMINAR E CRIAR


![image](https://github.com/user-attachments/assets/4ba93949-a3c3-4964-891e-1dfeaaea92f0)

CRIAR INDEXAÇÃO VETORIAL


![image](https://github.com/user-attachments/assets/7cc439a8-c4a8-4d5b-8279-44dd769f0fe3)

Neste momento, o modelo está pegando parte desses textos e transformando o texto em um array de numeros que vira um vetor. 
Quando eu fizer uma pergunta que contenha dentro de algum vetor, o modelo seleciona este contexto e retorna a resposta no chat. 

![image](https://github.com/user-attachments/assets/3d510dcb-db92-4ee2-b90d-971e8834a115)

![image](https://github.com/user-attachments/assets/7eac3036-c2d1-44de-88da-855f53447a01)

![image](https://github.com/user-attachments/assets/125fe5df-b2ba-4a49-a29e-e8b4a235c6dc)

![image](https://github.com/user-attachments/assets/a10cdfaf-ba42-4806-a182-e2b6c5ef1ae4)

![image](https://github.com/user-attachments/assets/e693ae7b-cf27-42e4-9ae5-f292b53926fc)

CLIQUE EM DADOS + INDICES NA ABA ESQUERDA

![image](https://github.com/user-attachments/assets/c57abafd-4751-44c9-8fd4-f61f34574925)

VOLTE EM PLAYGROUND + EXPERIMENTE O PLAYGROUND DO CHAT


![image](https://github.com/user-attachments/assets/5a0ea738-ecc8-4320-9411-373109cc8ed6)

VAMOS FAZER ALGUMAS PERGUNTAS 

Tenho uma aula do Professor Fagner entre os três documentos, por isso perguntei sobre o que se tratou na aula.


![image](https://github.com/user-attachments/assets/169da5b7-d606-4271-b23d-95fdc1e5fb4d)

Agora pedi para criar um relatório do que foi passado na aula que é toda por slides. 

![image](https://github.com/user-attachments/assets/f3b1aae6-1ec4-4b45-8e05-47a33388933a)

![image](https://github.com/user-attachments/assets/83f390ad-235a-4672-a4ec-7802025a7bf1)

![image](https://github.com/user-attachments/assets/17b0bcf7-2189-46e1-bbfa-e0f9687eb7f5)

![image](https://github.com/user-attachments/assets/4334c5eb-cc78-4d15-b726-1bfa3270dbed)


<h1> DEPLOYMENT DA APLICAÇÃO </h1>

Podemos ir além e implementar a solução como um aplicativo. 


![image](https://github.com/user-attachments/assets/df42d6d9-131b-458d-96d6-a95a98d6f16f)

![image](https://github.com/user-attachments/assets/24955708-b563-4ca0-b64b-53d02ac66f44)

* O meu não deu pra implantar porque não havia como escolher o local, vou criar novamente escolhendo outra região. O professor do bootcamp implementou com a região Sweden Central e o meu estava automaticamente, com Central US. Então como melhoria, poderia recriar o projeto trocando as regiões.

* Voltei para o playground e fiz mais algumas interações.


![image](https://github.com/user-attachments/assets/d64ea614-fd23-4ad5-aeb1-a8151d8941d8)

![image](https://github.com/user-attachments/assets/7e7db074-a645-4159-bbba-18aabcbd183f)

![image](https://github.com/user-attachments/assets/9e578ad9-9483-4f96-8774-ee6836355a16)

![image](https://github.com/user-attachments/assets/4470ddcb-6376-4d73-9e19-2122f8c2d401)

![image](https://github.com/user-attachments/assets/8b406805-a095-4491-89f6-cb540c1b1ef0)

![image](https://github.com/user-attachments/assets/251eca93-86a9-4e35-967d-e7be474d9de1)

Espero ter ajudado! Valeu!

<h1> EXCLUA SEU GRUPO DE RECURSOS </h1>




