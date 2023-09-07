# Install guide Hackintosh

## Pre Install
1. Baixar arquivos necessários
     - [Python](https://www.python.org/downloads/)
     - [EFI Base](https://github.com/luchina-gabriel?tab=repositories)
     - [ProperTree](https://github.com/corpnewt/ProperTree)
     - [MountEFI](https://github.com/corpnewt/ProperTree)
     - [genSMBIOS](https://github.com/corpnewt/ProperTree)
     - [OpenCore Packager](https://github.com/chris1111/OpenCore-Packager)
     - [ACPIca](https://github.com/acpica/acpica/)
     - Kexts necessárias não incluídas

2. Instale o Python (marcar a opção de `ADD Python to PATH`)
3. Formatar o flashdisk em fat32
4. Baixar Recovery
5. Gerar a SMBIOS
6. Gerar SSDT Tables
7. Gerar SysReport

 ### [Pos Install](https://dortania.github.io/OpenCore-Post-Install/#how-to-follow-this-guide)
 - [Mapear Portas USB](https://dortania.github.io/OpenCore-Post-Install/usb/intel-mapping/intel.html#Intel-usb-mapping)
 - [Corrigir `Built-in` das Placas de Redes](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#fixing-en0)
 - [Configurar Áudio](https://dortania.github.io/OpenCore-Post-Install/universal/audio.html#finding-your-layout-id)
 - [Configurar Som de Inicio](https://dortania.github.io/OpenCore-Post-Install/cosmetic/gui.html#setting-up-boot-chime-with-audiodxe)
 -  [Boot sem Pendrive](https://dortania.github.io/OpenCore-Post-Install/universal/oc2hdd.html#grabbing-opencore-off-the-usb)
 - [Corrigir CPU Name](https://github.com/corpnewt/CPU-Name)
 - [Corrigir problemas de Sleep](https://dortania.github.io/OpenCore-Post-Install/universal/sleep.html#preparations)
 - Ajustes estéticos no `config.plist`
     - `PickerAtributes → 17` - Modo Gráfico Open Core
     - `PickerMode → External` - Modo gráfico Open Core
     - `PollAppleHotKeys → True` - Habilita atalhos de boot no teclado como nos macs Originais
     - `PickerVariant → Auto` - Tema dos ícones do menu do Open Core
     - `HideAuxiliary → True` - Exibe somente os discos de SO no menu do Open Core (Para exibir as demais opções, pressione espaço e habilite `PollAppleHotKeys`
     - `Timeout → 5` - Tempo em segundos que o menu do Open Core vai ficar aberto
     - `ShowPicker → false` - Oculta o menu do Open Core
     - `LauncherOption → Full` - Migração da EFI para o disco do PC
     - `RequestBootVarRouting → True`  - Migração da EFI para o disco do PC
     - `ScanPolicy → 2687747` → Oculta os discos de Windows do menu de boot do Open Core

