<div align="center">
  
  <br />
  <h1 align="center">L U M I N A</h1>
  
  <p align="center">
    <b>Controle de brilho e calibração de cor de monitores para Windows.</b>
  </p>
  
  <p align="center">
    <a href="https://github.com/phdev2/Lumina/releases"><img src="https://img.shields.io/badge/Plataforma-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Platform" /></a>
    <a href="https://github.com/phdev2/Lumina/releases"><img src="https://img.shields.io/github/downloads/phdev2/Lumina/total?style=for-the-badge&color=2EA043&cache=bust1" alt="Downloads" /></a>
    <img src="https://img.shields.io/badge/.NET_8.0-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" alt=".NET 8" />
  </p>
  
  <br/>

  <p align="center">
    <img src="https://i.ibb.co/7tf1zv4K/image.png" alt="Painel Principal" width="250"/>
    &nbsp;&nbsp;&nbsp;&nbsp;
    <img src="https://i.ibb.co/rRhYvZFG/image.png" alt="Configurações Avançadas" width="250"/>
    &nbsp;&nbsp;&nbsp;&nbsp;
    <img src="https://i.ibb.co/gb44jJkC/image.png" alt="Seletor de Cores" width="250"/>
  </p>

  <br/><br/>
</div>

> **Lumina** é um utilitário leve e direto ao ponto que opera silenciosamente na bandeja do sistema. Seu objetivo central é fornecer ajuste imediato do brilho físico e calibração fina das cores do monitor via software, eliminando a dependência de menus físicos (OSD) dos displays.

---

### Principais Recursos

| Arquitetura & UX | Controle de Imagem |
| :--- | :--- |
| **Eficiência Máxima:** Interface minimalista em WPF. Baixíssimo consumo de RAM e CPU. | **Controle de Hardware:** Altera o nível de brilho nativo do painel. |
| **Acesso Imediato:** Reside na bandeja do sistema para invocação rápida. | **Calibração Avançada:** Níveis RGB, temperatura de cor e curva de gama. |
| **Gestão de Perfis:** Alternância instantânea entre configurações (Leitura, Filmes, Jogos). | **Contraste Dinâmico:** Ajuste fino de sombras e realces. |

---

### Download e Execução

O Lumina é autossuficiente e distribuído em formatos otimizados, sem exigir dependências externas pesadas.

1. Navegue até a seção [Releases](https://github.com/phdev2/Lumina/releases).
2. Faça o download da versão desejada (`LuminaInstaller.exe` para instalação automática ou `Lumina_Portable.exe` para uso direto).
3. Execute o aplicativo. Ele será inicializado silenciosamente na bandeja do sistema (próximo ao relógio).

---

### Segurança e Privacidade

O Lumina foi projetado sob o princípio de total transparência e respeito à máquina do usuário:

* **100% Offline:** O software é destituído de módulos de telemetria, não se comunica com a internet e não requer acesso de rede para operar.
* **Transparência de Execução:** O executável é compilado de forma limpa, empacotado sem dependências de terceiros, permitindo auditoria clara por qualquer software de segurança moderno.
* **Privilégios Restritos:** A aplicação se atém estritamente às APIs gráficas do Windows e ao protocolo DDC/CI, não instalando drivers em anel kernel e não solicitando elevação de privilégios de administrador.

---

### Arquitetura Subjacente

A comunicação com o hardware é efetivada por meio da tecnologia **DDC/CI** *(Display Data Channel Command Interface)*, transmitindo comandos I2C de forma direta para a controladora do monitor. As modificações de perfil de cor e curvas de gama são aplicadas através de injeção direta em nível de sistema operacional via `GDI32.dll`, assegurando estabilidade em tela cheia e transições isentas de latência.

<br/>

<div align="center">
  <sub>Construído por <a href="https://github.com/phdev2">phdev</a></sub>
</div>
