# Projeto 04 - Landing page responsiva

Landing page desenvolvida durante o curso de Front-end da Dankicode. O projeto simula o site de uma clínica, com navegação por seções, apresentação de serviços, tratamentos, vídeos, depoimentos, redes sociais e formulário de contato.

O foco do exercício foi praticar a construção de uma página institucional responsiva usando HTML, CSS e JavaScript, além da integração de um formulário com PHP e PHPMailer.

## Funcionalidades

- Layout responsivo para desktop e dispositivos móveis.
- Menu desktop e menu mobile com abertura e fechamento animados.
- Navegação suave entre as seções da página.
- Carrosséis responsivos para o mosaico de imagens, tratamentos e depoimentos.
- Validação básica dos campos do formulário no navegador.
- Envio dos dados do formulário por `POST` para um script PHP via AJAX.
- Envio de e-mail usando SMTP e a biblioteca PHPMailer.

## Tecnologias

- HTML5
- CSS3
- JavaScript
- jQuery
- Slick Carousel
- PHP
- PHPMailer

## Estrutura do projeto

```text
.
├── index.html                 # Página principal
├── css/
│   ├── style.css              # Estilos da página
│   └── slick.css              # Estilos do Slick Carousel
├── js/
│   ├── jquery.js              # Biblioteca jQuery
│   ├── menu-responsivo.js     # Comportamento do menu mobile
│   ├── menuScroll.js          # Rolagem suave do menu
│   ├── slides.js              # Configuração dos carrosséis
│   └── slick.js               # Biblioteca Slick Carousel
├── imagens/                   # Logos, ícones e imagens da página
├── contactform/
│   ├── contactform.js         # Validação e envio assíncrono do formulário
│   └── contactform.php        # Processamento e envio do e-mail
└── classes/
    ├── Mail.class.php         # Classe auxiliar de e-mail
    └── phpmailer/             # Arquivos da biblioteca PHPMailer
```

## Como executar

### Apenas visualizar a página

Como a página principal é estática, é possível abrir `index.html` diretamente no navegador. Nesse modo, os elementos HTML, CSS e JavaScript podem ser visualizados, mas o formulário de contato não funcionará corretamente porque depende do PHP e de um servidor SMTP.

### Executar com PHP

Para testar o projeto completo, use um servidor local com suporte a PHP, como XAMPP, WAMP ou o servidor embutido do PHP:

```bash
php -S localhost:8000
```

Depois, acesse [http://localhost:8000](http://localhost:8000) no navegador.

O comando deve ser executado na raiz do projeto, no mesmo diretório do arquivo `index.html`.

## Configuração do formulário

Antes de usar o formulário em um ambiente real:

1. Abra `contactform/contactform.php`.
2. Configure o servidor SMTP, a porta, o usuário, a senha e o endereço destinatário.
3. Substitua as credenciais atualmente configuradas por variáveis de ambiente ou por uma configuração fora do controle de versão.
4. Nunca publique senhas ou credenciais SMTP no repositório.

O formulário envia os campos `nome`, `email`, `telefone` e `mensagem`. O processamento atual usa PHPMailer e requer que a hospedagem permita conexões SMTP.

## Observações

- Não há etapa de build nem gerenciador de dependências obrigatório para executar a interface.
- As bibliotecas JavaScript e os estilos do Slick estão incluídos localmente no projeto.
- O conteúdo textual da página ainda contém textos demonstrativos, como `Lorem ipsum`, e pode ser substituído por conteúdo real.
- O envio de e-mail deve ser testado em um ambiente configurado com SMTP válido antes da publicação.

## Capturas de tela

![Captura de tela 1](https://user-images.githubusercontent.com/69223872/166522475-d3e603a7-ff6b-4f64-8081-59524f5416aa.png)
![Captura de tela 2](https://user-images.githubusercontent.com/69223872/166522487-367aa61a-7e18-459e-b2dd-585bbf2b0c09.png)
![Captura de tela 3](https://user-images.githubusercontent.com/69223872/166522492-89ff3497-e371-452d-9eca-d16da3aba26a.png)
![Captura de tela 4](https://user-images.githubusercontent.com/69223872/166522495-f4ec3764-734e-47a5-ae5f-8a1e52038de1.png)
![Captura de tela 5](https://user-images.githubusercontent.com/69223872/166522496-daca0acc-03b9-4285-a4b4-1e496839250f.png)
![Captura de tela 6](https://user-images.githubusercontent.com/69223872/166522500-a632a56c-d32c-4c2e-80bd-310e6c03ddce.png)
