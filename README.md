<div align="center"> 
<img src = "https://github.com/marcos-willian00/NLW-Unite-Pass.in/assets/152074631/f18226e3-fe8c-4a9e-b11e-f2c1839b541c" width = "300px">
</div>

## Pass.in

O pass.in é um aplicação voltada a gestão de participantes em eventos presenciais.

Nela o organizador pode cadastrar um evento e abrir uma página publica de inscrição.

Os participantes inscritos podem emitir uma credencial para check-in no dia do evento.

O sistema fará uma scan da credencial do participante para liberar sua entrada no evento.

## Requisitos Funcionais

- [✔️] O organizador deve poder cadastrar um novo evento;
- [✔️] O organizador deve poder visualizar os dados de um evento;
- [✔️] O organizador deve poder visualizar a lista de participantes;
- [✔️] O organizador deve poder se inscrever em um evento;
- [✔️] O organizador deve poder visualizar seu crachá de inscrição;
- [✔️] O organizador deve poder realizar check-in no evento;

## Regras de Negócio

- [✔️] O participante só pode se inscrever em um evento uma única vez;
- [✔️] O participante só pode se inscrever em eventos com vagas disponíveis;
- [✔️] O participante só pode realizar check-in em um evento uma única vez;

## Requisitos Não-funcionais

- [✔️] O check-in no evento será realizado através de um QRCode;

## Execução do Pass.in

### 1. Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:

- Você instalou a versão mais recente do NodeJS
  - Se sim, pode prosseguir
  - Se não, visite o site do [NodeJS](https://nodejs.org/en) e faça a instalação!

- Instalação das dependências do projeto
  - Antes de realizar os proximos comandos instale as dependências do projeto, isso vai garantir que ele funcione!
  - Este comando vai instalar todas as dependências de uma só vez!

  ```
  npm install
  ```

### 2. Seed

```
npx prisma seed
```

### 3. Executar em modo de desenvolvimento

```
npm run dev
```

### 4. Executar em modo de produção

- Para converter a aplicação TypeScript e gerar a aplicação JavaScript:
  ```
  npm run build
  ```
- Para rodar a aplicação JavaScript:
  ```
  npm start
  ```

### 5. Executar migrations

```
npm run db:migrate
```

### 6. Executar o Prisma Studio

```
npm run db:studio
```

### 7. Teste da aplicação

- Caso queira testar a aplicação e suas funcionalidades sem adentrar muito ao código acesse o swagger do pass.in!
  
- No navegador(quando a aplicação estiver rodando), visite a seguinte URL:
```
http://localhost:3333/docs
```
