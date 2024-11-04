<div align="center">
             <img src="docs/images/OC-Patcher.png" alt="OpenCore Patcher Logo" width="256" />
             <h1>OpenCore Legacy Patcher</h1>
</div>

Um projeto baseado em Python que gira em torno de [Acidanthera's OpenCorePkg](https://github.com/acidanthera/OpenCorePkg) and [Lilu](https://github.com/acidanthera/Lilu) tanto para executar quanto para desbloquear recursos no macOS em Macs suportados e não suportados.

"O principal objetivo do nosso projeto é dar uma nova vida aos Macs que não são mais suportados pela Apple, permitindo a instalação e o uso do macOS Big Sur e versões mais recentes em máquinas tão antigas quanto 2007"
----------

![GitHub all releases](https://img.shields.io/github/downloads/dortania/OpenCore-Legacy-Patcher/total?color=white&style=plastic) ![GitHub top language](https://img.shields.io/github/languages/top/dortania/OpenCore-Legacy-Patcher?color=4B8BBE&style=plastic) ![Discord](https://img.shields.io/discord/417165963327176704?color=7289da&label=discord&style=plastic)

----------

Recursos notáveis do OpenCore Legacy Patcher:

* Suporte para macOS Big Sur, Monterey, Ventura, Sonoma e Sequoia
* Atualizações de sistema nativas Over the Air (OTA)
* Suporta Macs Penryn e mais novos
* Suporte total para Wi-Fi WPA e Hotspot Pessoal em chipsets sem fio BCM943224 e mais novos
* Proteção de Integridade do Sistema, FileVault 2, Inicialização Segura .im4m e Vaulting
* Inicialização em Recovery OS, Modo Seguro e Modo de Usuário Único em sistemas operacionais não nativos
* Desbloqueia recursos como Sidecar e AirPlay para Mac mesmo em Macs nativos
* Habilita gerenciamento de energia SATA e NVMe aprimorado em dispositivos de armazenamento não Apple
* Nenhum patch de firmware necessário (ou seja, patching de ROM APFS)
* Aceleração gráfica para GPUs Metal e não Metal

----------

Nota: Apenas instalações limpas e atualizações são suportadas. Instalações do macOS Big Sur já patchadas com outros patchers, como [Patched Sur](https://github.com/BenSova/Patched-Sur) ou [bigmac](https://github.com/StarPlayrX/bigmac), não pode ser usado devido à integridade do arquivo quebrada com snapshots APFS e SIP.

* Você pode, no entanto, reinstalar o macOS com este patcher e manter seus dados originais.

Nota 2: Atualmente, o OpenCore Legacy Patcher suporta oficialmente o patching para executar o macOS Big Sur através de instalações do Sonoma. Para sistemas operacionais mais antigos, o OpenCore pode funcionar; no entanto, o suporte atualmente não é fornecido pela Dortania.

* Para suporte ao macOS Mojave e Catalina, recomendamos o uso de [dosdude1's patchers](http://dosdude1.com)

## Começando

Para começar a usar o projeto, por favor, veja nosso guia detalhado:

* [OpenCore Legacy Patcher Guide](https://dortania.github.io/OpenCore-Legacy-Patcher/)

## Suporte

Este projeto é oferecido na condição AS-IS, não garantimos suporte para quaisquer problemas que possam surgir. No entanto, há um servidor comunitário com outros usuários e desenvolvedores apaixonados que podem ajudá-lo:

* [OpenCore Patcher Paradise Discord Server](https://discord.gg/rqdPgH8xSN)
 * Lembre-se de que o servidor do Discord é mantido pela comunidade, então pedimos a todos que sejam respeitosos.
 * Por favor, revise nossa documentação sobre [how to debug with OpenCore](https://dortania.github.io/OpenCore-Legacy-Patcher/DEBUG.html) reunir informações importantes para ajudar outros com a resolução de problemas.

## Executando a partir do código-fonte

Para executar o projeto a partir do código-fonte, veja aqui: [Build and run from source](./SOURCE.md)

## Creditos

* [Acidanthera](https://github.com/Acidanthera)
  * OpenCorePkg, assim como muitos dos kexts e ferramentas principais
* [DhinakG](https://github.com/DhinakG)
  * Principal coautor
* [Khronokernel](https://github.com/Khronokernel)
  * Principal coautor
* [Ausdauersportler](https://github.com/Ausdauersportler)
  * Patch de atualização de GPUs Metal para iMacs e documentação
  * Grande quantidade de ajuda com depuração e sugestões de código
* [vit9696](https://github.com/vit9696)
  * Quantidade infinita de ajuda na resolução de problemas, determinação de correções e escrita de patches
* [ASentientBot](https://github.com/ASentientBot), [EduCovas](https://github.com/educovas) e [ASentientHedgehog](https://github.com/moosethegoose2213)
  * Conjunto de patches de aceleração legado e documentação, [Moraea Organization](https://github.com/moraea)
* [cdf](https://github.com/cdf)
  * Mac Pro no conjunto de patches OpenCore e documentação
  * [Innie](https://github.com/cdf/Innie) and [NightShiftEnabler](https://github.com/cdf/NightShiftEnabler)
* [Syncretic](https://forums.macrumors.com/members/syncretic.1173816/)
  * [AAAMouSSE](https://forums.macrumors.com/threads/mp3-1-others-sse-4-2-emulation-to-enable-amd-metal-driver.2206682/), [telemetrap](https://forums.macrumors.com/threads/mp3-1-others-sse-4-2-emulation-to-enable-amd-metal-driver.2206682/post-28447707) and [SurPlus](https://github.com/reenigneorcim/SurPlus)
* [dosdude1](https://github.com/dosdude1)
  * Autor principal do [original GUI](https://github.com/dortania/OCLP-GUI)
  * Desenvolvimento de patchers anteriores, delineando muito do que precisa ser corrigido
* [parrotgeek1](https://github.com/parrotgeek1)
  * [VMM Patch Set](https://github.com/dortania/OpenCore-Legacy-Patcher/blob/4a8f61a01da72b38a4b2250386cc4b497a31a839/payloads/Config/config.plist#L1222-L1281)
* [BarryKN](https://github.com/BarryKN)
  * Desenvolvimento de patchers anteriores, delineando muito do que precisa ser corrigido
* [mario_bros_tech](https://github.com/mariobrostech) e o resto do Discord de Macs Não Suportados
  * Catalisador que iniciou o OpenCore Legacy Patcher
* [arter97](https://github.com/arter97/)
  * [SimpleMSR](https://github.com/arter97/SimpleMSR/) desativar a limitação de firmware em MacBooks Nehalem+ sem baterias
* [Mr.Macintosh](https://mrmacintosh.com)
  * Horas intermináveis ajudando a arquitetar e solucionar problemas em muitas partes do projeto
* [flagers](https://github.com/flagersgit)
  * Auxiliar na pesquisa e desenvolvimento do driver da Nvidia Web
* [joevt](https://github.com/joevt)
  * [FixPCIeLinkrate](https://github.com/joevt/joevtApps)
* [Jazzzny](https://github.com/Jazzzny)
  * Pesquisa e várias contribuições para o projeto
  * Pesquisa e desenvolvimento de UEFI Legacy XHCI
  * Pesquisa e desenvolvimento de NVIDIA OpenCL
  * Pesquisa e desenvolvimento de ` MacBook5,2 `
  * LegacyKeyboardInjector
  * Patch de Ethernet Aquantia pré-Ivy Bridge
  * Patch de Photo Booth não-Metal para Monterey+
  * Desenvolvimento de GUI e Backend
  * UI do Atualizador
  * UI do Downloader do macOS
  * UI do Downloader
  * Probing do Top Case USB
  * Patch de root para desenvolvedores
  * Implementação de Vaulting
  * Pesquisa Helios 3802 do macOS 15
  * Pesquisa de bootx64.efi UEFI
  * Pesquisa de build universal2
  * Várias contribuições para a documentação
  * Usuários incríveis que gentilmente doaram hardware:
  * [JohnD](https://forums.macrumors.com/members/johnd.53633/) - 2013 Mac Pro
  * [SpiGAndromeda](https://github.com/SpiGAndromeda) - AMD Vega 64
  * [turbomacs](https://github.com/turbomacs) - 2014 5k iMac
  * [vinaypundith](https://forums.macrumors.com/members/vinaypundith.1212357/) - MacBook7,1
   * [ThatStella7922](https://github.com/ThatStella7922) - 2017 13" MacBook Pro (A1708)
  * zephar - 2008 Mac Pro
  * jazo97 - 2011 15" MacBook Pro
   * E outros (entre em contato se esquecemos de você!)
 * Comunidades MacRumors e Mac não suportados
  * Testes intermináveis e relatórios de problemas
  * Apple
  * para macOS e muitos dos kexts, frameworks e outros binários que reimplementamos em sistemas operacionais mais novos
