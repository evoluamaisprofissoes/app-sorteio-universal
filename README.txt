SORTEIO UNIVERSAL | VERSÃO ESTÁTICA

COMO USAR
1. Abra admin.html no navegador (Chrome ou Edge recomendado).
2. Configure a campanha, cadastre os prêmios e quantidades.
3. Cadastre participantes manualmente ou importe Excel/CSV.
4. Vá à aba SORTEIO e revele um ganhador por vez.
5. Exporte os resultados em CSV e o backup completo em JSON.

PUBLICAR NO GITHUB PAGES
1. Envie toda esta pasta para a raiz do repositório GitHub.
2. No painel, configure a campanha e clique em BAIXAR ARQUIVO DO SITE.
3. Coloque o arquivo campaign.json baixado na mesma pasta do index.html e publique novamente.
4. O site público exibirá a campanha e os prêmios definidos no campaign.json.

IMPORTANTE SOBRE OS DADOS
- Não há Firebase, Supabase, banco de dados ou servidor.
- Participantes, resultados e alterações administrativas existem somente na memória da aba do navegador.
- Atualizar ou fechar a aba apaga a sessão. Exporte o backup JSON para guardar participantes, campanha e resultados.
- O arquivo campaign.json contém apenas os dados públicos da campanha e dos prêmios. Não contém participantes nem ganhadores.
- O site público é uma página de divulgação. O cadastro e a importação dos participantes são feitos no painel local do organizador.
- A importação Excel usa SheetJS por CDN e precisa de internet para carregar a biblioteca. CSV funciona sem essa biblioteca.
- O sorteio escolhe o ganhador com crypto.getRandomValues quando disponível, antes de iniciar a animação. A animação apenas revela a pessoa já escolhida.

PLANILHA
Colunas aceitas: nome (obrigatória), telefone ou whatsapp (opcional), email (opcional).
Duplicidades de nome + telefone são ignoradas.
