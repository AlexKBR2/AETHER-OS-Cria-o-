# Arquitetura inicial

**Status:** proposta em avaliação — não é uma decisão final de implementação.

## Objetivo

Construir um desktop Linux voltado prioritariamente a jogos, mas adequado também a navegação, produtividade, multimídia e tarefas cotidianas.

## Componentes a avaliar

| Camada | Direção inicial | Observações |
|---|---|---|
| Base do sistema | Fedora / Universal Blue / Bazzite como referências | Comparar manutenção, atualização, rollback, codecs, drivers e liberdade de customização antes de escolher. |
| Kernel | Kernel Linux mantido pela distribuição-base | Evitar patches próprios sem necessidade demonstrada. |
| Ambiente desktop | KDE Plasma | Permite personalização ampla e uma experiência familiar. |
| Gráficos AMD | Mesa, AMDGPU e Vulkan | Validar suporte por GPU e versão; não presumir que todos os recursos estejam disponíveis em hardware antigo. |
| Jogos | Steam, Proton, DXVK e VKD3D-Proton | Compatibilidade varia por jogo, DRM e antitrapaça. |
| Outros launchers | Heroic e Lutris, conforme necessidade | Avaliar manutenção, segurança e experiência. |
| Aplicativos Windows | Wine e Bottles | Não substituem compatibilidade nativa nem garantem execução de todo aplicativo. |

## Princípios de arquitetura

- Preferir componentes mantidos por projetos reconhecidos.
- Evitar duplicação desnecessária de serviços e ferramentas.
- Separar claramente componentes do sistema, aplicativos e configurações do usuário.
- Planejar atualização e recuperação antes de personalizar profundamente a base.
- Não escolher a distribuição-base apenas por benchmarks isolados.

## Decisões ainda abertas

1. Distribuição-base e modelo de atualização.
2. Imagem imutável ou tradicional.
3. Estratégia de drivers e kernels.
4. Ferramenta de construção da imagem.
5. Política de codecs e repositórios adicionais.
6. Estratégia de recuperação e rollback.
7. Escopo e tecnologia do painel próprio de configurações.
