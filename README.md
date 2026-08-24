<div align="center">
  <h1>Lumina</h1>
  <p><b>Controle de brilho e calibração de cor de monitores para Windows.</b></p>
  
  [![Platform](https://img.shields.io/badge/Plataforma-Windows-blue?style=flat-square&logo=windows)](https://github.com/phdev2/Lumina/releases)
  [![Downloads](https://img.shields.io/github/downloads/phdev2/Lumina/total?style=flat-square&color=success)](https://github.com/phdev2/Lumina/releases)
</div>

<br/>

Lumina é um utilitário leve e direto ao ponto que roda na bandeja do sistema. O objetivo principal é permitir o ajuste rápido do brilho e a calibração avançada de cores do monitor via software, dispensando a necessidade de utilizar os botões físicos da tela.

<div align="center">
  <img src="https://i.ibb.co/7tf1zv4K/image.png" alt="Screenshot do Lumina 1" width="600"/><br/><br/>
  <img src="https://i.ibb.co/rRhYvZFG/image.png" alt="Screenshot do Lumina 2" width="600"/><br/><br/>
  <img src="https://i.ibb.co/gb44jJkC/image.png" alt="Screenshot do Lumina 3" width="600"/>
</div>

## Principais Recursos

- **Controle de Hardware:** Altera o nível de brilho físico do monitor de forma nativa.
- **Calibração Avançada:** Suporte a ajustes de níveis RGB, temperatura de cor e curva de gama.
- **Sombras e Realces:** Ajuste fino de contraste para evitar fadiga visual em diferentes ambientes de iluminação.
- **Gestão de Perfis:** Sistema de presets (padrões) para salvar e alternar entre diferentes configurações instantaneamente.
- **Eficiência:** Interface construída em WPF e otimizada para manter baixo consumo de RAM e CPU.

## Download e Execução

O Lumina é autossuficiente e distribuído em formato portátil, sem exigir instalações complexas.

1. Acesse a seção [Releases](https://github.com/phdev2/Lumina/releases).
2. Faça o download da versão mais recente (`Lumina.exe`).
3. Execute o aplicativo. Ele será inicializado silenciosamente na bandeja do sistema (perto do relógio).

## Segurança e Privacidade

O Lumina foi projetado sob o princípio de total transparência e respeito à privacidade do usuário:

- **100% Offline:** O aplicativo não possui código de telemetria, não se comunica com a internet e não requer acesso a rede para funcionar.
- **Transparência de Execução:** O arquivo executável é empacotado de forma limpa e é distribuído livre de dependências obscuras de terceiros, podendo ser livremente verificado por qualquer software antivírus antes de sua execução.
- **Zero Permissões Suspeitas:** O software se atém rigorosamente às APIs gráficas do Windows e ao protocolo DDC/CI, sem instalar drivers ocultos, serviços persistentes em background (além do próprio processo quando aberto) ou solicitar privilégios além dos necessários para gerenciar a imagem da tela.

## Detalhes Técnicos

A comunicação com o hardware é realizada por meio da tecnologia DDC/CI (Display Data Channel Command Interface), enviando comandos I2C diretamente para o controlador do monitor. Para as modificações de cor, o aplicativo altera as rampas de gama em nível de sistema operacional (via GDI32), garantindo estabilidade e transições sem travamentos.

---
Desenvolvido por [phdev](https://github.com/phdev2).
