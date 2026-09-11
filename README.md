# meus-desafios-criativos
Atue como um especialista em N8N.
Crie uma automação para identificar em uma planilha de Excel (armazenada na raiz do Google Drive com o nome "Vara_Civil.xlsx") os e-mails pendentes, disparar mensagens personalizadas via Gmail e atualizar a planilha com a data e o status do envio.

Público:
Servidores e responsáveis pelas Varas Cíveis do TJMG cadastradas na planilha.

Ferramentas envolvidas:
Google Drive, Google Sheets (ou leitura de arquivo Excel via Drive) e Gmail.

Fluxo:
1. Disparar a execução a partir de um agendamento ou data/hora definida.
2. Localizar e ler o arquivo "Vara_Civil.xlsx" na raiz do Google Drive.
3. Filtrar apenas as linhas cujo status de envio ainda esteja pendente ou vazio.
4. Para cada registro elegível, disparar um e-mail via Gmail com cabeçalho/assunto e corpo personalizados com o nome da respectiva Vara Cível.
5. Atualizar a linha correspondente na planilha preenchendo a coluna "Status" com a confirmação de envio e a coluna "Data" com o registro de data/hora atual.

Regras:
1. O e-mail deve ter o cabeçalho e saudação personalizados individualmente para cada Vara Cível (ex.: "À Vara Cível de [Comarca/Nome da Vara]").
2. Apenas e-mails com status diferente de "Enviado" devem ser processados (evitar envios duplicados).
3. Registrar na planilha o status imediato do envio e a data/hora exata da operação.

Explique quais nós do N8N devem ser utilizados e a lógica de funcionamento do workflow.
