# Repertório do Casamento

Página única (`index.html`) com o setlist do casamento e as observações de execução para a cantora.

## O que tem na página

- **Chegada dos convidados**: setlist numerado, com a indicação de tocar tudo acústico e em volume baixo, e a transição para a cerimônia (encerrar quando o cerimonial avisar dos 5 minutos e fazer uma pausa em silêncio).
- **Cerimônia**: os oito momentos na ordem (padrinhos, pais, noivo, florista, noiva, alianças, assinaturas, saída do casal), cada um com a música e as observações. Os momentos ainda sem música (entrada dos pais e assinaturas) aparecem como "A definir" até alguém escolher.
- **Restaurante**: setlist numerado.
- **Copiar lista em texto**: copia tudo, já formatado, para colar no WhatsApp ou no e-mail.

## Adicionar ou editar músicas

1. Toque em **Adicionar ou editar músicas**.
2. Use **+ Adicionar música** na parte do roteiro onde ela deve tocar. Preencha a música, o artista ou a versão e as observações para a cantora.
3. Também dá para editar, mudar a ordem (Subir/Descer) ou remover músicas.
4. Toque em **Salvar**. Até salvar, nada muda para quem abre o link.

As músicas adicionadas aparecem com a etiqueta "Adicionada em dd/mm", assim a cantora vê o que é novo.

### Onde as alterações ficam salvas

- **Publicada como Artifact no claude.ai**: ao salvar, a página publica uma nova versão de si mesma. Todo mundo que abrir o link vê a lista atualizada. Para salvar, a pessoa precisa ter acesso de edição ao artifact. Quem só visualiza, como a cantora, vê a lista sem os botões de edição.
- **Aberta direto do arquivo ou de outro site** (GitHub Pages, por exemplo): as alterações ficam salvas só no navegador de quem editou. Nesse caso, use "Copiar lista em texto" para enviar a lista.

## Estrutura

Tudo fica em `index.html`:

- `<script id="repertorio-dados">`: a lista em JSON (seções, momentos, músicas e observações). Para mudar a lista base, edite esse bloco.
- `<style id="estilo">`: o visual, com tema claro e escuro.
- `<script id="logica">`: renderização, edição e salvamento.
