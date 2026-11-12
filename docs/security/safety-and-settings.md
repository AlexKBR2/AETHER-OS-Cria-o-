# Segurança, configurações e proteção contra erros

## Objetivo

Oferecer muitas opções sem transformar o painel de configurações em uma fonte de instabilidade. A regra central é:

**Máxima liberdade para o usuário. Máxima proteção contra erros.**

## Níveis de configuração

### Básico
Opções comuns, com linguagem simples e valores recomendados.

### Personalizado
Controles adicionais, explicações mais detalhadas e possibilidade de salvar perfis.

### Avançado
Opções técnicas, unidades, pré-requisitos, limites suportados e indicação clara dos riscos.

O usuário deve conseguir pesquisar qualquer configuração disponível. A interface deve explicar o que a opção altera, quando é útil e quais efeitos adversos são possíveis.

## Regras de segurança

1. **Detecção de hardware:** mostrar apenas opções compatíveis com o equipamento detectado.
2. **Validação:** verificar valores, dependências e limites antes de aplicar.
3. **Reversibilidade:** registrar o valor anterior e oferecer desfazer sempre que tecnicamente possível.
4. **Perfis:** permitir salvar, comparar e restaurar configurações.
5. **Mudanças críticas:** exigir confirmação explícita e explicar se será necessário reiniciar.
6. **Recuperação:** planejar snapshots, rollback e um modo de recuperação antes de mudanças estruturais.
7. **Privilégios mínimos:** solicitar permissões administrativas somente para a ação que realmente precisar delas.
8. **Auditoria local:** manter histórico compreensível das alterações, sem coletar dados desnecessários.
9. **Falha segura:** se uma validação falhar, não aplicar a alteração.
10. **Limites de hardware:** não permitir valores fora das especificações suportadas pelo fabricante ou firmware.

## Áreas que exigem cautela especial

- Frequência, tensão, potência e temperatura de CPU/GPU.
- Memória, timings e tensão de RAM.
- Firmware, BIOS/UEFI e microcódigo.
- Partições, sistemas de arquivos e carregador de inicialização.
- Drivers, módulos de kernel e parâmetros de boot.
- Firewall, permissões, serviços e autenticação.
- Atualizações e alterações na imagem do sistema.

## Limitações

Nenhum painel consegue garantir que toda alteração será segura em qualquer equipamento. Falhas físicas, firmware defeituoso, bugs de drivers, falta de energia e incompatibilidades podem causar problemas. A proteção deve reduzir riscos e facilitar recuperação, sem prometer risco zero.

## Requisitos para cada configuração

Cada opção avançada deverá documentar:
- Nome e descrição em linguagem simples.
- Hardware e versões compatíveis.
- Valor padrão e faixa permitida.
- Unidade de medida.
- Benefício esperado.
- Riscos e efeitos colaterais.
- Método de validação.
- Método de reversão.
- Necessidade de reinicialização.
