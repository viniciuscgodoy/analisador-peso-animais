# Analisador de Ganho de Peso dos Animais

Aplicação web para análise de ganho de peso diário de animais através de planilhas CSV/Excel.

## 🚀 Funcionalidades

- Upload de arquivos CSV e Excel (.xlsx, .xls)
- Cálculo automático de ganho de peso diário por animal
- Visualização em gráfico de dispersão
- Filtros por pasto/local
- Estatísticas detalhadas
- Interface responsiva

## 📁 Estrutura do Projeto

```
analisador-ganho-peso-animais/
├── index.html          # Arquivo principal da aplicação
├── README.md           # Documentação do projeto
├── assets/             # Pasta para recursos (opcional)
│   ├── screenshots/    # Screenshots da aplicação
│   └── examples/       # Arquivos de exemplo
└── docs/               # Documentação adicional (opcional)
```

## 🛠️ Tecnologias Utilizadas

- **HTML5/CSS3/JavaScript**: Base da aplicação
- **React 18**: Interface do usuário
- **Recharts**: Visualização de dados
- **Tailwind CSS**: Estilização
- **XLSX**: Processamento de planilhas Excel
- **PapaParse**: Processamento de arquivos CSV
- **Lodash**: Utilitários JavaScript
- **Babel**: Transformação JSX

## 📋 Pré-requisitos

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexão com internet (para carregar bibliotecas via CDN)

## 🚀 Como Usar

1. **Clone ou baixe o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/analisador-ganho-peso-animais.git
   cd analisador-ganho-peso-animais
   ```

2. **Abra o arquivo no navegador:**
   - Dê duplo clique em `index.html`, ou
   - Use um servidor local (recomendado):
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   
   # Node.js (se tiver o live-server instalado)
   npx live-server
   ```

3. **Acesse no navegador:**
   - Arquivo local: `file:///caminho/para/index.html`
   - Servidor local: `http://localhost:8000`

## 📊 Formato dos Dados

A planilha deve conter as seguintes colunas (nomes não são case-sensitive):

| Coluna | Descrição | Exemplo |
|--------|-----------|---------|
| ANIMAL | Identificação do animal | "001", "Touro123" |
| DATA_PESAGEM | Data da pesagem | "01/01/2024", "2024-01-01" |
| PESO | Peso em kg | 450.5, 480 |
| LOCAL | Pasto/Local | "Pasto A", "Curral 1" |
| SX | Sexo (opcional) | "M", "F" |

### Exemplo de dados CSV:
```csv
ANIMAL,DATA_PESAGEM,PESO,LOCAL,SX
001,01/01/2024,450,Pasto A,M
001,15/01/2024,465,Pasto A,M
002,01/01/2024,380,Pasto B,F
002,15/01/2024,392,Pasto B,F
```

## 🌐 GitHub Pages

Para hospedar gratuitamente no GitHub Pages:

1. Vá para Settings → Pages
2. Source: "Deploy from a branch"
3. Branch: "main" ou "master"
4. Pasta: "/ (root)"
5. Salve

Sua aplicação ficará disponível em: `https://seu-usuario.github.io/analisador-ganho-peso-animais/`

## 🔧 Resolução de Problemas

### Bibliotecas não carregam
- Verifique sua conexão com internet
- Desative bloqueadores de anúncios/scripts
- Tente usar um servidor local em vez de abrir diretamente o arquivo

### Erro ao processar planilha
- Verifique se as colunas têm os nomes corretos
- Certifique-se que as datas estão em formato válido
- Verifique se há pelo menos 2 pesagens por animal

### Gráfico não aparece
- Certifique-se que há dados processados
- Verifique se o filtro por pasto não está removendo todos os dados

## 📝 Como Contribuir

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 👨‍💻 Autor

Seu Nome - [@viniciuscgodoy](https://github.com/viniciuscgodoy)

## 🙏 Agradecimentos

- React Team pela biblioteca React
- Recharts pela biblioteca de gráficos
- Tailwind CSS pelo framework de CSS
- Todos os desenvolvedores das bibliotecas utilizadas
