# mautic-integracao-elementor
Integração Fácil de formulário Mautic com Formulário do Elementor


Olá, para quem usa um Elementor e quer integrar com os formulários do Mautic encontrei uma solução de contorno para a falta de compatibilidade nativa.

## Aviso

Esse é um procedimento "workaround" / alternativo para quem não quer usar nenhum plugin adicional.

## Procedimento: 

1. Crie seu formulário normalmente no Mautic 
2. Anote os Field HTML Name de cada elemento / ou na Página de Edição do Formulário vá em Manual Copy e veja os names dos componentes (name="mauticform[meu_nome]")
3. Pegue a sua URL do Mautic (Geralmente http://[SITE ou IP]/form/submit
4. No Form do Elementor coloque as labels dos campos com o mesmo NAME do form no Mautic Ex: Label: mauticform[meu_nome]
5. Selecione para não mostrar a Label para o usuário
6. Adicione um campo hidden no Form Elementor com a Label mauticform[formId] e em Advanced: Default Value o ID do seu formulário no Mautic
7. Adicione a ação : Enviar Webhook, e coloque a sua URL do mautic (Geralmente http://[SITE ou IP]/form/submit

Pronto, seu formulário Elementor está integrado ao Mautic

As labels no Elementor ficarão assim:

![alt text](https://github.com/thaina128/mautic-integracao-elementor/blob/master/form-elementor.png?raw=true)


## Abraço a todos!
