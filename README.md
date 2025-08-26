# Projeto: GuiaTur - Aplicativo de Turismo Regional
## Sobre
Este projeto tem como objetivo desenvolver um aplicativo mobile completo para centralizar e organizar informações sobre turismo em regiões do interior de São Paulo. O GuiaTur busca facilitar o acesso a roteiros turísticos, eventos e experiências que hoje estão dispersos em redes sociais e páginas isoladas, promovendo o turismo rural, cultural e corporativo de forma acessível e colaborativa.

## Repositório
### O projeto é dividido em dois repositórios principais:
- **guiatur-frontend**: Responsável pelo aplicativo mobile usando React Native e interface do usuário.
- **guiatur-backend**: Responsável pelas APIs, lógica de negócio, autenticação e integração com banco de dados usando Node.js.

## Ferramentas Utilizadas
- **Git**: Controle de versão. `v2.44.0`
- **VSCode**: Editor de código. `v1.89.0`
- **Node.js**: Ambiente de execução. `v18.17.0`
- **Expo CLI**: Desenvolvimento React Native. `v6.3.0`
- **Postman**: Testes de APIs. `v10.18.0`
- **Figma**: Prototipagem da interface.
- **Jira Software**: Gestão de tarefas e sprints.

## Tecnologias
### Frontend (Mobile)
- **React Native** `v0.72.0`
- **Expo** `v49.0.0`
- **React Navigation** `v6.1.7`
- **Styled Components** `v6.0.7`
- **Axios** `v1.5.0`
- **React Hook Form** `v7.45.4`
- **TypeScript** `v5.1.6`
  
### Backend
- **Node.js** `v18.17.0`
- **Express.js** `v4.18.2`
- **MongoDB** `v6.0`
- **Mongoose** `v7.5.0`
- **JWT** `v9.0.2`
- **Bcrypt** `v5.1.0`
- **Multer** `v1.4.5`
- **Cors** `v2.8.5`

### Ferramentas de Desenvolvimento
- **ESLint**: Linting de código
- **Prettier**: Formatação de código
- **Jest**: Testes unitários
- **Nodemon**: Hot reload para desenvolvimento

---

## 🌐 Links Úteis
Aqui estão alguns links importantes para facilitar o acesso às ferramentas e informações relacionadas ao projeto:

- [Jira Software](https://guiatur.atlassian.net/jira/software/projects/GT/boards/1)
- [Figma - Protótipos](https://www.figma.com/design/RbU7KABp5S96A9UwncgBXQ/Untitled?node-id=0-1&p=f&t=9jWoWvVagVbmnrFf-0)
---

## Fluxo de Trabalho: Commits e Branches
Este projeto utiliza um fluxo de trabalho baseado em Git Flow para garantir que as contribuições sejam bem organizadas e colaborativas. Cada desenvolvedor trabalhará em sua própria branch de feature e seguirá as diretrizes para commits e pull requests.

###  Criação de Branches

O projeto utiliza a seguinte convenção de branches:

- **main**: Branch principal com código estável em produção
- **develop**: Branch de desenvolvimento com últimas features integradas
- **feature/nome-da-feature**: Branches para desenvolvimento de novas funcionalidades
- **bugfix/nome-do-bug**: Branches para correção de bugs
- **hotfix/nome-do-hotfix**: Branches para correções críticas em produção

**Exemplo de criação de branch**:
```bash
git checkout develop
git pull origin develop
git checkout -b feature/cadastro-roteiros
```

### Commits
As mensagens de commit devem seguir o padrão Conventional Commits para facilitar a automação e entendimento do histórico:

**Formato**: `tipo(escopo): descrição`

**Tipos disponíveis**:
- `feat`: Nova funcionalidade
- `fix`: Correção de bug
- `docs`: Alterações na documentação
- `style`: Mudanças de formatação/estilo
- `refactor`: Refatoração de código
- `test`: Adição ou correção de testes
- `chore`: Mudanças em ferramentas, configurações, etc.

**Exemplos**:
```bash
feat(auth): adicionar sistema de login com JWT
fix(routes): corrigir erro 404 na busca de roteiros
docs(readme): atualizar instruções de instalação
style(components): ajustar indentação nos componentes
refactor(api): reorganizar estrutura das controllers
test(auth): adicionar testes para autenticação
chore(deps): atualizar dependências do React Native
```

## Pull Requests

### Processo de Pull Request

1. **Finalize sua feature** na branch correspondente
2. **Atualize sua branch** com a develop:
   ```bash
   git checkout develop
   git pull origin develop
   git checkout feature/sua-feature
   git rebase develop
   ```
3. **Execute os testes** e verifique se tudo está funcionando
4. **Crie o Pull Request** para a branch `develop`
5. **Preencha o template** de PR com:
   - Descrição clara do que foi implementado
   - Tipo de mudança (bugfix, feature, etc.)
   - Como testar as mudanças
   - Screenshots (se aplicável)
6. **Aguarde revisão** de pelo menos um membro da equipe
7. **Realize ajustes** se necessário baseado no feedback

### Template de Pull Request
```markdown
## Tipo de Mudança
- [ ] Bug fix
- [ ] Nova feature
- [ ] Breaking change
- [ ] Documentação

## Descrição
Descreva as mudanças implementadas...

## Como Testar
1. Execute `npm install`
2. Execute `npm start`
3. Navegue para...

## Screenshots (se aplicável)
Adicione screenshots das mudanças visuais...

## Checklist
- [ ] Meu código segue o style guide do projeto
- [ ] Realizei self-review do código
- [ ] Adicionei comentários em partes complexas
- [ ] Meus changes não geram novos warnings
- [ ] Adicionei testes que provam que minha correção/feature funciona
- [ ] Testes unitários passam localmente
```

---

## 🧠 Rotina de Reuniões e Gestão do Projeto

Este projeto utiliza metodologia Scrum adaptada para desenvolvimento mobile, com sprints de 2 semanas e reuniões periódicas para manter a equipe alinhada.

## Reuniões

#### Daily Standup
- **Frequência**: Segunda, quarta e sexta-feira
- **Duração**: 15 minutos
- **Horário**: 09:00
- **Formato**:
  - O que fiz desde a última daily?
  - O que farei até a próxima?
  - Estou com algum impedimento?

#### Sprint Planning
- **Frequência**: A cada 2 semanas (início da sprint)
- **Duração**: 2 horas
- **Objetivo**:
  - Planejar tarefas da sprint
  - Estimar story points
  - Definir meta da sprint
  - Alocar responsáveis

#### Sprint Review
- **Frequência**: A cada 2 semanas (final da sprint)
- **Duração**: 1 hora
- **Objetivo**:
  - Demonstrar funcionalidades entregues
  - Coletar feedback do Product Owner
  - Atualizar backlog baseado no feedback

#### Sprint Retrospective
- **Frequência**: Após cada Sprint Review
- **Duração**: 45 minutos
- **Objetivo**:
  - Refletir sobre o que funcionou bem
  - Identificar pontos de melhoria
  - Definir ações para próxima sprint

### Ferramentas Utilizadas
- **Jira**: Organização de backlog, sprints e acompanhamento
- **GitHub**: Versionamento e revisão de código
- **Discord**: Reuniões síncronas e comunicação
- **Confluence**: Documentação e atas de reunião

> 💡 *As reuniões são adaptáveis conforme disponibilidade da equipe e podem ser ajustadas baseadas nas necessidades do projeto.*

---

# Guia de Estilo - GuiaTur

Este projeto segue padrões rigorosos de estilo para manter a organização, legibilidade e padronização do código entre as equipes de frontend e backend.

---

## 📁 Convenções de Nomeação

### Arquivos e Pastas

#### Frontend (React Native)
```
src/
├── components/           # Componentes reutilizáveis
│   ├── Button/
│   │   ├── index.tsx
│   │   └── styles.ts
│   └── Header/
├── screens/             # Telas do aplicativo
│   ├── HomeScreen/
│   ├── LoginScreen/
│   └── ProfileScreen/
├── services/            # Chamadas para API
│   ├── api.ts
│   ├── authService.ts
│   └── routesService.ts
├── hooks/               # Custom hooks
│   ├── useAuth.ts
│   └── useLocalStorage.ts
├── utils/               # Funções utilitárias
│   ├── formatters.ts
│   ├── validators.ts
│   └── constants.ts
├── types/               # Definições TypeScript
│   ├── auth.ts
│   ├── routes.ts
│   └── user.ts
└── assets/              # Imagens, ícones, etc.
    ├── images/
    ├── icons/
    └── fonts/
```

#### Backend (Node.js)
```
src/
├── controllers/         # Lógica dos endpoints
│   ├── authController.js
│   ├── routesController.js
│   └── userController.js
├── models/              # Modelos do banco de dados
│   ├── User.js
│   ├── Route.js
│   └── Event.js
├── routes/              # Definição das rotas
│   ├── authRoutes.js
│   ├── routeRoutes.js
│   └── userRoutes.js
├── middleware/          # Middlewares personalizados
│   ├── authMiddleware.js
│   ├── errorMiddleware.js
│   └── uploadMiddleware.js
├── services/            # Lógica de negócio
│   ├── authService.js
│   ├── emailService.js
│   └── imageService.js
├── utils/               # Funções utilitárias
│   ├── helpers.js
│   ├── validators.js
│   └── constants.js
├── config/              # Configurações
│   ├── database.js
│   ├── cloudinary.js
│   └── env.js
└── tests/               # Testes automatizados
    ├── unit/
    ├── integration/
    └── fixtures/
```

### Variáveis e Funções

#### JavaScript/TypeScript (Frontend)
- Use `camelCase` para variáveis e funções
- Use `PascalCase` para componentes e classes
- Use `UPPER_SNAKE_CASE` para constantes

```typescript
// ✅ BOA
const userName = 'João';
const isLoggedIn = true;
const API_BASE_URL = 'https://api.guiatur.com';

const LoginScreen = () => {};
class UserService {}

function calculateDistance(lat1: number, lon1: number) {}
const handleSubmitForm = async () => {};

// ❌ RUIM
const user_name = 'João';
const IsLoggedIn = true;
const apibaseurl = 'https://api.guiatur.com';

const loginScreen = () => {};
class userService {}
```

#### JavaScript (Backend)
- Use `camelCase` para variáveis e funções
- Use `PascalCase` para classes e construtores
- Use `UPPER_SNAKE_CASE` para constantes de ambiente

```javascript
// ✅ BOA
const userEmail = req.body.email;
const isValidUser = await validateUser(userId);
const JWT_SECRET = process.env.JWT_SECRET;

class UserController {
  async createUser(req, res) {}
}

function generateToken(payload) {}
const authenticateUser = async (email, password) => {};

// ❌ RUIM
const user_email = req.body.email;
const IsValidUser = await validateUser(userId);
const jwt_secret = process.env.JWT_SECRET;

class userController {}
```

### Componentes React Native

```typescript
// ✅ BOA - Estrutura de componente
import React from 'react';
import { View, Text, TouchableOpacity } from 'react-native';
import { styles } from './styles';
import { ButtonProps } from '../../types/components';

const CustomButton: React.FC<ButtonProps> = ({ 
  title, 
  onPress, 
  variant = 'primary' 
}) => {
  return (
    <TouchableOpacity 
      style={[styles.button, styles[variant]]} 
      onPress={onPress}
    >
      <Text style={styles.buttonText}>{title}</Text>
    </TouchableOpacity>
  );
};

export default CustomButton;

// ❌ RUIM
const customButton = ({ title, onPress }) => {
  return (
    <TouchableOpacity onPress={onPress}>
      <Text>{title}</Text>
    </TouchableOpacity>
  );
};
```

### Rotas da API (Backend)

```javascript
// ✅ BOA - Nomenclatura de rotas REST
GET    /api/v1/routes           // Listar roteiros
GET    /api/v1/routes/:id       // Buscar roteiro específico
POST   /api/v1/routes           // Criar roteiro
PUT    /api/v1/routes/:id       // Atualizar roteiro
DELETE /api/v1/routes/:id       // Deletar roteiro

GET    /api/v1/users/profile    // Perfil do usuário
POST   /api/v1/auth/login       // Login
POST   /api/v1/auth/register    // Registro
POST   /api/v1/auth/logout      // Logout

// ❌ RUIM
GET    /getRoutes
POST   /createNewRoute
GET    /user_profile
POST   /doLogin
```

## 🎨 Convenções de Estilo

### Indentação e Formatação
- Use **2 espaços** para indentação (não tabs)
- Máximo de **80 caracteres** por linha
- Use **Prettier** para formatação automática
- Use **ESLint** para linting

### Imports
```typescript
// ✅ BOA - Ordem dos imports
// 1. Bibliotecas externas
import React, { useState, useEffect } from 'react';
import { View, Text } from 'react-native';
import axios from 'axios';

// 2. Imports internos (services, utils, etc.)
import { authService } from '../services/authService';
import { formatDate } from '../utils/formatters';

// 3. Imports locais (components, styles)
import CustomButton from './CustomButton';
import { styles } from './styles';

// 4. Imports de tipos (sempre por último)
import { User, Route } from '../types';

// ❌ RUIM - Imports desorganizados
import { styles } from './styles';
import React from 'react';
import { User } from '../types';
import axios from 'axios';
import CustomButton from './CustomButton';
```

### Comentários
```typescript
// ✅ BOA - Comentários úteis
/**
 * Calcula a distância entre dois pontos geográficos
 * @param lat1 Latitude do primeiro ponto
 * @param lon1 Longitude do primeiro ponto
 * @param lat2 Latitude do segundo ponto
 * @param lon2 Longitude do segundo ponto
 * @returns Distância em quilômetros
 */
function calculateDistance(lat1: number, lon1: number, lat2: number, lon2: number): number {
  // Fórmula de Haversine para calcular distância
  const R = 6371; // Raio da Terra em km
  // ... implementação
}

// TODO: Implementar cache para melhorar performance
// FIXME: Corrigir bug de validação de email

// ❌ RUIM - Comentários desnecessários
// Incrementa o contador
counter++;

// Esta função faz login
function login() {}
```

### Tratamento de Erros

#### Frontend
```typescript
// ✅ BOA - Tratamento de erros consistente
const loginUser = async (email: string, password: string) => {
  try {
    const response = await authService.login(email, password);
    return { success: true, data: response.data };
  } catch (error) {
    console.error('Login error:', error);
    
    if (error.response?.status === 401) {
      return { success: false, message: 'Credenciais inválidas' };
    }
    
    return { success: false, message: 'Erro interno do servidor' };
  }
};

// ❌ RUIM
const loginUser = async (email, password) => {
  const response = await authService.login(email, password);
  return response.data;
};
```

#### Backend
```javascript
// ✅ BOA - Middleware de erro padronizado
const errorHandler = (err, req, res, next) => {
  console.error(err.stack);

  if (err.name === 'ValidationError') {
    return res.status(400).json({
      success: false,
      message: 'Dados de entrada inválidos',
      errors: err.errors
    });
  }

  if (err.name === 'JsonWebTokenError') {
    return res.status(401).json({
      success: false,
      message: 'Token inválido'
    });
  }

  res.status(500).json({
    success: false,
    message: 'Erro interno do servidor'
  });
};

// ❌ RUIM
app.use((err, req, res, next) => {
  res.status(500).send('Algo deu errado!');
});
```

## 📱 Convenções Específicas do React Native

### Estrutura de Estilos
```typescript
// ✅ BOA - Organização de estilos
import { StyleSheet } from 'react-native';

export const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#FFFFFF',
    paddingHorizontal: 16,
  },
  
  header: {
    height: 60,
    justifyContent: 'center',
    alignItems: 'center',
    borderBottomWidth: 1,
    borderBottomColor: '#E5E5E5',
  },
  
  title: {
    fontSize: 18,
    fontWeight: '600',
    color: '#333333',
  },
  
  button: {
    height: 48,
    backgroundColor: '#007AFF',
    borderRadius: 8,
    justifyContent: 'center',
    alignItems: 'center',
    marginTop: 16,
  },
  
  buttonText: {
    color: '#FFFFFF',
    fontSize: 16,
    fontWeight: '500',
  },
});

// ❌ RUIM - Estilos inline e desorganizados
<View style={{ flex: 1, backgroundColor: 'white', padding: 20 }}>
  <Text style={{ fontSize: 20, color: 'black' }}>Título</Text>
</View>
```

### Gerenciamento de Estado
```typescript
// ✅ BOA - Hook personalizado para estado
import { useState, useEffect } from 'react';
import { authService } from '../services/authService';

export const useAuth = () => {
  const [user, setUser] = useState(null);
  const [isLoading, setIsLoading] = useState(true);
  const [error, setError] = useState(null);

  const login = async (email: string, password: string) => {
    try {
      setIsLoading(true);
      setError(null);
      
      const response = await authService.login(email, password);
      setUser(response.user);
      
      return { success: true };
    } catch (err) {
      setError('Erro ao fazer login');
      return { success: false, message: err.message };
    } finally {
      setIsLoading(false);
    }
  };

  return { user, isLoading, error, login };
};

// ❌ RUIM - Estado espalhado pelo componente
const LoginScreen = () => {
  const [user, setUser] = useState(null);
  const [loading, setLoading] = useState(false);
  const [err, setErr] = useState('');
  
  // lógica misturada com UI
};
```

## 🔧 Configuração do Ambiente

### ESLint (.eslintrc.js)
```javascript
module.exports = {
  root: true,
  extends: [
    '@react-native-community',
    'eslint:recommended',
    '@typescript-eslint/recommended',
  ],
  parser: '@typescript-eslint/parser',
  plugins: ['@typescript-eslint'],
  rules: {
    'indent': ['error', 2],
    'quotes': ['error', 'single'],
    'semi': ['error', 'always'],
    'comma-dangle': ['error', 'always-multiline'],
    'no-unused-vars': 'error',
    'no-console': 'warn',
    '@typescript-eslint/no-explicit-any': 'error',
  },
};
```

### Prettier (.prettierrc)
```json
{
  "semi": true,
  "trailingComma": "es5",
  "singleQuote": true,
  "printWidth": 80,
  "tabWidth": 2,
  "useTabs": false
}
```

## 📚 Recursos e Referências

- [React Native Style Guide](https://github.com/callstack/react-native-paper)
- [Node.js Best Practices](https://github.com/goldbergyoni/nodebestpractices)
- [TypeScript Do's and Don'ts](https://www.typescriptlang.org/docs/handbook/declaration-files/do-s-and-don-ts.html)
- [Conventional Commits](https://www.conventionalcommits.org/)
- [REST API Design Guidelines](https://github.com/microsoft/api-guidelines)

---

> 💡 *Este guia de estilo é um documento vivo e deve ser atualizado conforme o projeto evolui. Todos os membros da equipe são encorajados a sugerir melhorias.*
