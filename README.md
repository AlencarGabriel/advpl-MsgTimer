# advpl-MsgTimer
Função AdvPL de mensagens (Alert, Info, Stop, Success, YesNo e NoYes) com Timer para fechamento automático

## Implementação
Compilar o fonte MsgTimer no seu RPO e chamar via chamada de função de usuário `U_MsgTimer()`

## Futuras implementações
- [ ] [Implementar Conout quando IsBlind](https://github.com/AlencarGabriel/advpl-MsgTimer/issues/1)

## [Reportar problemas ou sugerir melhorias](https://github.com/AlencarGabriel/advpl-MsgTimer/issues)

## Colaborar
Assim como meu objetivo é ajudar aqueles que precisam, caso você faça uma melhoria ou encontre algum problema no projeto, fique a vontade para ajustar e me mandar seu [Pull Request](https://github.com/AlencarGabriel/advpl-MsgTimer/pulls), estarei avaliando e com certeza sendo útil estará disponível e farei uma dedicação.

---

# Documentação

### Lista de Parâmetros:
  
Ordem | Parâmetro | Tipo        | Opicional? | Default     | Descrição
------|-----------|-------------|------------|-------------|-------------------------------
1     | nSeconds  | Numeric     | Sim        | 0           | Tempo em segundos que a mensagem será exibida antes de ser fechada
2     | cMensagem | Characters  | Sim        | " "         | Descrição da mensagem [TEXT or HTML Formats]
3     | cTitulo   | Characters  | Sim        | " "         | Título da mensagem [TEXT or HTML Formats]
4     | cIcone    | Characters  | Sim        | MT_IINFO    | Ícone formato MT_I[ICON OF MESSAGE] ou RESOURCE compilados
5     | nTipo     | Numeric     | Sim        | MT_TDEFAULT | Tipo de mensagem formato MT_T[TYPE OF MESSAGE]


> **Importante!** Uso de HTML no Título e/ou Mensagem pode ocasionar problemas de dimensionamento nas mensagens.
