# ChatFiles

## Deploy with Vercel

<p align="center">
<a href="https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fguangzhengli%2FChatFiles&env=NEXT_PUBLIC_CHAT_FILES_UPLOAD_PATH,SUPABASE_SERVICE_ROLE_KEY,SUPABASE_URL&envDescription=Have%20a%20conversation%20with%20files&envLink=https%3A%2F%2Fgithub.com%2Fguangzhengli%2FChatFiles%2Fblob%2Fmain%2Fdoc%2Fenv-vars.md&demo-title=ChatFiles&demo-description=Have%20a%20conversation%20with%20files&demo-url=https%3A%2F%2Fchat-file.vercel.app%2F"><img src="https://vercel.com/button" alt="Deploy with Vercel"/></a>
</p>

> this repository use [LangchainJS](https://github.com/hwchase17/langchainjs), based on [Chatbot-ui](https://github.com/mckaywrigley/chatbot-ui)

Technical architecture

![Embedding](./doc/Embedding.png)

Product screenshot.

![ChatFiles](./doc/chatfiles.png)

**Upload your file and have a conversation with it.**


## How to use it

### Init Vector DB
[Crate a vector db on Supabase](doc/vectordb/supabase.md)

### How to run locally without limited
1. clone this repository.
2. create a .env file on root path.
3. set environment variables in .env file follow [doc/env-vars.md](doc/env-vars.md).

open browser with http://localhost:3000

## How to run locally
### chatfiles-ui

```shell
npm install
npm run dev
```

### How to deploy on vercel
1. Click the Deploy Button.
2. Set environment variables follow [doc/env-vars.md](doc/env-vars.md).
3. Pay attention to the NEXT_PUBLIC_CHAT_FILES_UPLOAD_PATH value must be /tmp.

## Feature

- [x] Chat with GPT-3.5
- [x] Chat with file by langchainjs and supabase vector db.




