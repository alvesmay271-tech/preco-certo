# Preço Certo — app instalável

App para celular e computador que ajuda profissionais autônomas e pequenos negócios a estimar preços, organizar produtos e criar orçamentos. Os arquivos funcionam sem conta: os dados são guardados somente no navegador/aparelho.

## Recursos desta versão

- **Calculadora de preços:** materiais, embalagem, tempo de trabalho e valor da hora, frete pago por unidade, desperdício, custos fixos rateados por volume, impostos, comissão, taxa de cartão/plataforma e margem desejada.
- **Formas de pagamento:** sugestões de taxa para Pix/dinheiro, débito, crédito e parcelado; altere as taxas para os valores do seu contrato.
- **Desconto seguro:** compara o desconto escolhido com a margem, exibe lucro estimado e preço mínimo para cobrir os custos.
- **Modelos por atividade:** lembretes de custos para confeitaria, artesanato, beleza, costura e prestação de serviços. Os exemplos são sugestões, sem valores automáticos.
- **Catálogo:** salva produtos/serviços, busca e ordena por preço, lucro e revisão, permite editar e manter histórico quando o preço muda.
- **Revisão de preços:** guarda uma data de revisão e mostra um aviso quando o app é aberto após o prazo; é um aviso local dentro do app, não uma notificação externa.
- **Orçamentos:** seleciona produtos e kits, define cliente, validade, forma de pagamento e observações; salva, copia para compartilhar ou imprime em PDF pelo navegador.
- **Kits e combos:** reúne itens do catálogo, estima preço com margem escolhida e permite usar o kit em orçamento.
- **Metas e cenários:** estima unidades para cobrir custos fixos e chegar a uma meta mensal; compara um preço alternativo.
- **Relatórios:** margem estimada, lucro por item, pendências de revisão e exportação CSV.
- **Backup:** exporta e restaura os dados num arquivo JSON. A importação substitui os dados que já estão no aparelho.
- **Migração:** ao abrir, tenta trazer o catálogo guardado pela versão anterior do Preço Certo no mesmo navegador.
- **PWA:** manifest, ícones e cache para instalar na tela inicial e abrir offline após a primeira visita.

## Instalar ou abrir

Para a instalação na tela inicial e o modo offline, hospede **todos** os arquivos desta pasta em HTTPS, acesse o `index.html` pelo navegador e use “Instalar app” (Android/Chrome) ou “Adicionar à Tela de Início” (iPhone/Safari). Service workers não rodam via `file://`. O arquivo HTML sozinho contém a calculadora e a interface; para instalação/offline, use a pasta completa, incluindo manifest, ícones e service worker.

## Precisão e limites

Todos os valores estimados são de apoio e dependem dos dados que você informar. O app não calcula automaticamente regimes tributários, obrigações, frete pago pelo cliente, descontos progressivos ou regras específicas da atividade. Confira custos e taxas reais e procure orientação contábil/tributária quando necessário. Não há pagamentos, assinaturas, conta ou sincronização entre aparelhos neste MVP.

Os dados ficam no armazenamento local do navegador. Se limpar os dados desse navegador, poderá perdê-los; baixe um backup JSON para transferir ou guardar uma cópia. A revisão de preço aparece como aviso ao abrir o app — não envia notificações fora dele.

## Ideia de receita (não ativada)

Uma versão futura poderia oferecer gratuitamente a calculadora básica e cobrar por recursos extras, como catálogo sincronizado, orçamentos com identidade visual, modelos avançados e relatórios. Esta versão **não recebe pagamentos** nem promete renda. Antes de cobrar, teste se as pessoas realmente pagariam e planeje um meio de pagamento seguro, políticas de privacidade, suporte e obrigações aplicáveis.
