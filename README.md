# Minhas Conversas — projeto Android

Este projeto cria um app Android com leitor offline e integração para receber arquivos `.txt` pelo menu Compartilhar/Abrir do Android.

## Gerar o APK sem programar
1. Baixe e extraia este ZIP.
2. Abra `https://github.com/new` e crie um repositório vazio.
3. Envie os arquivos e pastas deste projeto para o repositório.
4. A ação do GitHub em `.github/workflows/build-apk.yml` compila o projeto automaticamente.
5. Abra a aba **Actions**, selecione a execução mais recente e baixe o artefato **MinhasConversas-debug-apk**.
6. No Android, abra o APK baixado e permita a instalação desta fonte se o sistema pedir.

## Uso
No WhatsApp, exporte uma conversa **sem mídia** e toque em Compartilhar. Escolha **Minhas Conversas**. O app recebe o TXT e tenta abrir a conversa automaticamente.
Mídias: nesta primeira versão do app Android, o leitor web permite importar mídia manualmente na tela; a associação automática de arquivos compartilhados junto com o TXT ainda não está implementada.
Os dados são processados localmente. O app não solicita permissão de internet.

## Observação técnica
O ambiente em que este projeto foi preparado não tem Android SDK/Gradle instalado, então não foi possível compilar e validar um APK diretamente aqui. O workflow do GitHub Actions gera o APK usando o ambiente Android de compilação.
