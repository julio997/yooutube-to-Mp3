# YouTube para MP3 - WebApp

Uma aplicação web responsiva para converter vídeos do YouTube em arquivos MP3. Este projeto foi desenvolvido com HTML5, CSS3 e JavaScript puro, otimizado para funcionar como um aplicativo web progressivo (PWA) e pode ser facilmente convertido em um APK para Android.

## 🎯 Funcionalidades

- ✅ **Conversão de YouTube para MP3**: Cole um link e converta em segundos
- ✅ **Interface Responsiva**: Funciona perfeitamente em celulares, tablets e desktops
- ✅ **Armazenamento Local**: Salva seus downloads usando IndexedDB
- ✅ **Modo Offline**: Funciona offline após o primeiro carregamento (PWA)
- ✅ **Sem Dependências Externas**: Código puro, sem frameworks pesados
- ✅ **Compatível com Android**: Pode ser convertido em APK facilmente
- ✅ **Aviso Legal**: Mensagens claras sobre uso responsável

## 📱 Como Usar

### Via Navegador (Web)

1. **Abra o arquivo `index.html`** em seu navegador
2. **Cole um link do YouTube** no campo de entrada
3. **Clique em "Converter para MP3"**
4. **Aguarde a conversão** e o download será iniciado automaticamente
5. **Acesse seus downloads** na seção "Downloads Concluídos"

### Converter em APK (ApkCreator ou Web2APK)

#### Opção 1: Usando ApkCreator Online

1. Acesse [ApkCreator](https://www.apkcreator.com/) ou [Web2APK](https://www.web2apk.com/)
2. Clique em "Create APK"
3. Preencha os campos:
   - **App Name**: YouTube para MP3
   - **App URL**: Aponte para o arquivo `index.html` (você pode fazer upload dos arquivos em um servidor, ou usar um serviço como GitHub Pages)
   - **App Icon**: Selecione o arquivo `assets/icons/icon-192.png`
   - **App Package Name**: com.example.youtubetomp3
4. Clique em "Build APK"
5. Aguarde a compilação e baixe o arquivo `.apk`
6. Transfira para seu celular e instale

#### Opção 2: Usando GitHub Pages (Recomendado)

1. **Crie um repositório GitHub** com os arquivos do projeto
2. **Ative GitHub Pages** nas configurações do repositório
3. **Obtenha a URL** do seu site (ex: `https://seu-usuario.github.io/youtube-to-mp3`)
4. **Use essa URL** no ApkCreator

#### Opção 3: Usando um Servidor Web Local

Se quiser testar localmente antes de converter em APK:

```bash
# Com Python 3
python3 -m http.server 8000

# Com Node.js (se tiver instalado)
npx http-server
```

Então acesse `http://localhost:8000` no seu navegador.

## 📂 Estrutura do Projeto

```
YouTubeToMP3WebApp/
├── index.html              # Página principal
├── manifest.json           # Configuração PWA
├── service-worker.js       # Service Worker para offline
├── css/
│   └── styles.css         # Estilos responsivos
├── js/
│   ├── app.js             # Lógica principal
│   └── api.js             # Integração com APIs
└── assets/
    └── icons/             # Ícones para PWA e APK
```

## 🔧 Configuração de API

O aplicativo suporta múltiplas APIs de conversão:

### API Gratuita (Padrão)
- **Cobalt API**: Gratuita, sem autenticação
- Editável em `js/api.js` na seção `API_CONFIG`

### API Paga (Opcional)
- **RapidAPI**: Requer chave de API
- Para usar, obtenha uma chave em [RapidAPI - YouTube to MP3](https://rapidapi.com/marcocollatina/api/youtube-to-mp315)
- Insira a chave em `js/api.js`

## ⚙️ Instalação no Android

### Pré-requisitos
- Android 5.0 ou superior
- Permissão para instalar aplicativos de fontes desconhecidas

### Passos

1. **Baixe o arquivo APK** gerado
2. **Transfira para seu celular** (via USB, email, etc.)
3. **Abra o gerenciador de arquivos** do seu celular
4. **Localize o arquivo `.apk`** e toque para instalar
5. **Autorize a instalação** quando solicitado
6. **Pronto!** O app está instalado e pronto para usar

## ⚖️ Aviso Legal

Este aplicativo foi desenvolvido para fins educacionais e de uso pessoal. O usuário é o único responsável pelo conteúdo baixado.

**Importante:**
- Baixe apenas conteúdos que você tenha direito de usar
- Respeite os Termos de Serviço do YouTube
- Não viole direitos autorais
- Conteúdos próprios, livres de direitos ou com licença adequada são seguros para baixar

## 🛠️ Desenvolvimento

### Dependências
- Nenhuma! O projeto usa apenas HTML5, CSS3 e JavaScript puro

### Navegadores Suportados
- Chrome/Chromium 50+
- Firefox 45+
- Safari 10+
- Edge 15+

### Compatibilidade Android
- Android 5.0+ (para navegador)
- Android 6.0+ (para APK convertido)

## 📝 Licença

Este projeto é fornecido como está, para fins educacionais.

## 🤝 Contribuições

Sugestões e melhorias são bem-vindas! Você pode:
- Reportar bugs
- Sugerir novas funcionalidades
- Melhorar o código
- Traduzir para outros idiomas

## 📞 Suporte

Se encontrar problemas:

1. **Verifique sua conexão de internet**
2. **Limpe o cache do navegador**
3. **Tente em outro navegador**
4. **Verifique se a URL do YouTube é válida**

---

**Desenvolvido com ❤️ para Android**

Última atualização: 2026
