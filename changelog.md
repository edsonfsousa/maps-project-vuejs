{{#each releases}}
# {{title}}
[{{isoDate}}]

{{! lista de commits marcados como feature, utilize feature: ou Feature: }}
{{#commit-list 
  commits 
  heading='### Novas funcionalidades' 
{{/commit-list}}

{{! Lista com correções, para adicionar commit aqui utilize fix: ou Fix: }}
{{#commit-list 
  commits 
  heading='### Correções' 
{{/commit-list}}

{{! Lista com quebras de compatibilidade, utilize break: ou Break: }}
{{#commit-list 
  commits 
  heading='### Quebras de compatibilidade' 
{{/commit-list}}

{{/each}}