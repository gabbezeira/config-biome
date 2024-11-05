
# 🌿 Configuração Biome

Este repositório contém um arquivo de configuração de estilo para o [Biome](https://biomejs.dev/guides/getting-started/), uma poderosa ferramenta de formatação e linting para código. Siga as instruções abaixo para configurar rapidamente o Biome em seu projeto e garantir um código mais limpo e consistente.

---

## 🚀 Instalação do Biome

Para começar, instale o pacote Biome em seu projeto usando um dos seguintes gerenciadores de pacotes:

| Gerenciador de Pacotes                         | Comando                                                                                       |
|------------------------------------------------|-----------------------------------------------------------------------------------------------|
| ![npm](https://img.shields.io/badge/-npm-CB3837?logo=npm&logoColor=white)      | `npm install --save-dev --save-exact @biomejs/biome`                                         |
| ![yarn](https://img.shields.io/badge/-yarn-2C8EBB?logo=yarn&logoColor=white)   | `yarn add --dev --exact @biomejs/biome`                                                      |
| ![pnpm](https://img.shields.io/badge/-pnpm-F69220?logo=pnpm&logoColor=white)   | `pnpm add --save-dev --save-exact @biomejs/biome`                                            |
| ![bun](https://img.shields.io/badge/-bun-000000?logo=bun&logoColor=white)      | `bun add --dev --exact @biomejs/biome`                                                       |
| ![deno](https://img.shields.io/badge/-deno-000000?logo=deno&logoColor=white)   | `deno add --dev npm:@biomejs/biome`                                                          |

---

## 📄 Configuração

Baixe o arquivo de configuração `biome.json` diretamente para o diretório raiz do seu projeto. Esse arquivo contém as definições de estilo para garantir que seu código siga as diretrizes do Biome:

```bash
curl -O https://raw.githubusercontent.com/gabbezeira/config-biome/refs/heads/main/biome.json
```

---

## 🔧 Configuração do VS Code

Para uma integração completa no VS Code, siga estes passos:

1. Instale a extensão [Biome para VS Code](https://marketplace.visualstudio.com/items?itemName=biomejs.biome) ![VS Code](https://img.shields.io/badge/-VS%20Code-007ACC?logo=visual-studio-code&logoColor=white).
2. Adicione as seguintes configurações no seu `settings.json` para definir o Biome como o formatador padrão e configurar ações automáticas ao salvar:

   ```json
   "editor.defaultFormatter": "biomejs.biome",
   "editor.formatOnSave": true,
   "editor.codeActionsOnSave": {
      "source.organizeImports.biome": "explicit",
      "quickfix.biome": "explicit"
   }
   ```

---

## 🛠️ Uso

Após a instalação e configuração, utilize os comandos abaixo para formatar seu código e verificar problemas de linting:

- **Formatar o código**: `npx biome format .`
- **Verificar problemas de linting**: `npx biome lint .`

Para mais informações e comandos adicionais, consulte a [documentação do Biome](https://biomejs.dev/guides/getting-started/).

---

## 🎉 Contribuição

Contribuições são bem-vindas! Se desejar melhorar esta configuração ou adicionar novas funcionalidades, sinta-se à vontade para enviar um pull request.

## 📄 Licença

Este projeto está licenciado sob a Licença MIT.

---
