# Compatibilidade com jogos e aplicativos Windows

## Objetivo

Oferecer caminhos claros para executar jogos e aplicativos Windows no Linux, informando limitações sem prometer compatibilidade universal.

## Tecnologias a avaliar

- **Proton:** camada de compatibilidade usada principalmente com Steam.
- **Wine:** implementação de APIs do Windows para sistemas Unix-like.
- **DXVK:** tradução de Direct3D 9/10/11 para Vulkan.
- **VKD3D-Proton:** implementação de Direct3D 12 sobre Vulkan voltada a jogos.
- **Bottles:** gerenciamento de ambientes Wine.
- **Heroic Games Launcher e Lutris:** gerenciamento de bibliotecas e instaladores, conforme suporte atual.

## Limitações importantes

Podem existir bloqueios relacionados a:
- Antitrapaça que exige driver ou componente de kernel Windows.
- DRM e sistemas de proteção.
- Launchers e atualizadores proprietários.
- Drivers específicos e periféricos especializados.
- Aplicativos que dependem de serviços ou APIs não implementados.

Uma máquina virtual Windows pode ser considerada para casos específicos, mas desempenho 3D, acesso direto à GPU, licenciamento e antitrapaça têm limitações próprias.

## Política de testes

Para cada título ou aplicativo testado, registrar:
- Nome e versão.
- Loja/launcher.
- Hardware e driver gráfico.
- Versão do kernel, Wine/Proton e componentes relevantes.
- Configurações usadas.
- Resultado: funciona, funciona com ressalvas, não funciona ou não testado.
- Problemas observados e data do teste.

Não classificar algo como compatível com base apenas em relatos antigos ou em um único equipamento.
