# Luna

Assistente de voz local para Windows, com avatar Live2D, memória e chats de live. Tudo roda no seu PC.
Este repositório distribui o **Luna.exe**: o download fica em [Releases](../../releases/latest).

## Instalar

1. Baixe o `Luna-<versão>.zip` na versão mais recente em [Releases](../../releases/latest) e extraia a pasta inteira.
2. Instale o [Ollama](https://ollama.com), que é o motor do modelo de conversa.
3. Abra o `Luna.exe`. Na primeira vez ele cria o arquivo de configuração `.env` e abre o assistente, que:
   - confere a instalação;
   - mostra os modelos que faltam, cada um com o tamanho, e só baixa se você disser sim;
   - testa o microfone.
4. Chame "Luna" e ouça a resposta. O painel abre no navegador, com uma aba de Tutoriais.

## Requisitos

- Windows 10 ou 11.
- Ollama instalado.
- Cerca de 11 GB de modelos na primeira vez: conversa (Gemma, 9,6 GB), memória pelo sentido (639 MB),
  voz (642 MB) e reconhecimento de voz (Whisper, 142 MB).
- A placa de vídeo ajuda, mas não é obrigatória.
- O VTube Studio é opcional. O avatar no desktop precisa do Node.js e do Cubism Core da Live2D.
- A voz local (Kyutai Pocket TTS) pede que você aceite os termos em
  [huggingface.co/kyutai/pocket-tts](https://huggingface.co/kyutai/pocket-tts) e entre com `hf auth login`.

## Comandos

```
Luna.exe                       liga a Luna
Luna.exe diagnostico           confere a instalação
Luna.exe primeira-execucao     abre o assistente de novo (modelos e microfone)
Luna.exe --perfil live-vtube   as opções do launcher passam direto
```

## Privacidade

- Conversas, memória e traços ficam na pasta `data` do seu PC.
- Mensagens dos chats de YouTube, Twitch e Kick não são salvas.
- E-mail e agenda não entram na memória nem nos traços.

## Problemas e sugestões

Abra uma [issue](../../issues) com o que aconteceu e a saída de `Luna.exe diagnostico`.

## Créditos

Ver [CREDITOS.txt](CREDITOS.txt). Luna é um projeto bitcoin100treta.
