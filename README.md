# AI900LABAULA3
Análise de Sentimentos com Language Studio no Azure AI
Explorar o Estúdio de Fala
O serviço Azure AI Speech transcreve a fala em texto e o texto em fala audível. Você pode usar o AI Speech para criar um aplicativo que possa transcrever notas de reuniões ou gerar texto a partir da gravação de entrevistas.

Neste exercício, você experimentará os recursos do Azure AI Speech usando o Azure AI Speech Studio.

Criar um recurso de fala do Azure AI
Você pode usar o serviço de Fala criando um recurso de Fala ou um recurso de serviços de IA do Azure.

Neste exercício, você criará um recurso AI Speech, a menos que já tenha um recurso que possa usar.

Em outra guia do navegador, abra o Azure AI Speech Studio , entrando com sua conta da Microsoft.

Selecione Configurações e depois Crie um recurso. Configure-o com as seguintes configurações:

Nome do novo recurso: Insira um nome exclusivo.
Assinatura: sua assinatura do Azure.
Região: Selecione uma região suportada.
Nível de preços: FO gratuito (se disponível, caso contrário, selecione Padrão S0).
Grupo de recursos: Selecione ou crie um grupo de recursos com um nome exclusivo.
Selecione Criar recurso. Aguarde até que o recurso seja criado e selecione Usar recurso . A página Introdução à Fala é exibida.

Explore a fala para texto no Speech Studio
Selecione https://aka.ms/mslearn-speech-files para baixar o speech.zip. Abra a pasta.

Na página Introdução à fala, em Fala para texto, localize Fala em tempo real para texto . Selecione Experimente a fala em tempo real para texto.

Em Escolher arquivos de áudio, selecione Procurar arquivos e navegue até a pasta onde você salvou o arquivo. Selecione WhatAICanDo.m4a e depois Abrir.

O serviço Speech transcreve e exibe o texto em tempo real. Se você tiver áudio em seu computador, poderá ouvir a gravação enquanto o texto é transcrito.

Revise a saída, que deve ter reconhecido e transcrito com êxito o áudio em texto.

Neste exercício você criou um recurso AI Speech no Speech Studio. Em seguida, você usou o serviço de fala em texto em tempo real para transcrever uma gravação de áudio. Você pôde ver a transcrição do texto sendo gerada à medida que o arquivo de áudio era reproduzido.

Analise texto com Language Studio
Neste exercício, você explorará os recursos da linguagem Azure AI analisando alguns exemplos de avaliações de hotéis. Você usará o Language Studio para entender se as avaliações são em sua maioria positivas ou negativas.

O Processamento de Linguagem Natural (PNL) é um ramo da IA ​​que lida com a linguagem escrita e falada. Você pode usar a PNL para construir soluções que extraiam significado semântico de texto ou fala, ou que formulem respostas significativas em linguagem natural.

Por exemplo, suponha que a agência de viagens fictícia Margie's Travel incentive os clientes a enviar avaliações sobre estadias em hotéis. Você pode usar o serviço de idiomas para identificar frases-chave, determinar quais avaliações são positivas e quais são negativas ou analisar o texto da avaliação em busca de menções a entidades conhecidas, como locais ou pessoas.

O Azure AI Language Service inclui análise de texto e recursos de PNL. Isso inclui a identificação de frases-chave no texto e a classificação do texto com base no sentimento.

Crie um recurso de idioma
Você pode usar muitos recursos do Azure AI Language com um recurso de idioma ou de serviços do Azure AI. Existem alguns casos em que apenas um recurso Idioma pode ser usado. Para o exercício abaixo, utilizaremos um recurso Linguagem. Se ainda não o fez, crie um recurso de idioma na sua assinatura do Azure.

Em outra guia do navegador, abra o portal do Azure em https://portal.azure.com , entrando com a conta da Microsoft associada à sua assinatura do Azure.

Clique no botão ＋ Criar um recurso e pesquise Serviço de idioma. Selecione criar um plano de serviço de idiomas. Você será levado a uma página para selecionar recursos adicionais. Mantenha a seleção padrão e clique em Continuar para criar seu recurso.

Na página Criar Idioma, configure-o com as seguintes configurações:

Assinatura: sua assinatura do Azure.
Grupo de recursos: Selecione ou crie um grupo de recursos com um nome exclusivo.
Região: Leste dos EUA.
Nome: Insira um nome exclusivo.
Nível de preços: F0 grátis ou S se F0 grátis não estiver disponível
Ao marcar esta caixa, confirmo que li e compreendi todos os termos abaixo: Selecionado.
Selecione Revisar + criar e depois Criar e aguarde a conclusão da implantação.

Configure seu recurso no Azure AI Language Studio
Em outra guia do navegador, abra o Language Studio em https://language.cognitive.azure.com e entre.

Quando solicitado com Select an Azure resource , faça as seguintes configurações:

Diretório do Azure: diretório padrão, o diretório que você está usando
Assinatura do Azure: selecione a assinatura que você está usando
Tipo de recurso: Idioma
Nome do recurso: selecione o recurso de serviço de idioma que você acabou de criar
Em seguida, selecione Concluído.

Analise avaliações no Language Studio
Num navegador web, navegue até Language Studio em https://language.cognitive.azure.com.

Na página inicial Bem-vindo ao Language Studio, selecione a guia Classificar texto e, em seguida, selecione o bloco Analisar sentimento e extrair opiniões.

Em Selecionar idioma do texto, selecione Inglês.

Em Selecione seu recurso do Azure, selecione seu recurso.

Em Digite seu próprio texto, carregue um arquivo ou use um de nossos textos de exemplo, copie e cole a seguinte revisão:

Tired hotel with poor service
The Royal Hotel, London, United Kingdom
5/6/2018
This is an old hotel (has been around since 1950's) and the room furnishings are average - becoming a bit old now and require changing. The internet didn't work and had to come to one of their office rooms to check in for my flight home. The website says it's close to the British Museum, but it's too far to walk.
Marque a caixa para confirmar que a demonstração incorrerá em uso e poderá gerar custos e selecione Executar.

Revise a saída. Observe que o documento é analisado quanto ao sentimento, assim como cada frase. Selecione Frase 1 para mostrar a análise de sentimento dessa frase.

Observe que há um sentimento geral seguido por pontuações próximas a três categorias: pontuação positiva , pontuação neutra e pontuação negativa. Em cada uma das categorias é atribuída uma pontuação entre 0 e 1. Essas pontuações de confiança indicam a probabilidade do texto fornecido ser um sentimento específico.

Selecione a frase 1 novamente para fechar.

Role para cima para selecionar Limpar caixa de texto e copie e cole a seguinte revisão:

Good Hotel and staff
The Royal Hotel, London, UK
3/2/2018
Clean rooms, good service, great location near Buckingham Palace and Westminster Abbey, and so on. We thoroughly enjoyed our stay. The courtyard is very peaceful and we went to a restaurant which is part of the same group and is Indian ( West coast so plenty of fish) with a Michelin Star. We had the taster menu which was fabulous. The rooms were very well appointed with a kitchen, lounge, bedroom and enormous bathroom. Thoroughly recommended.
Selecione Executar. Revise o resultado e o sentimento e o nível de confiança.

Selecione Limpar caixa de texto novamente e copie e cole a seguinte revisão:

Very noisy and rooms are tiny The Lombard Hotel, San Francisco, USA 9/5/2018 Hotel is located on Lombard street which is a very busy SIX lane street directly off the Golden Gate Bridge. Traffic from early morning until late at night especially on weekends. Noise would not be so bad if rooms were better insulated but they are not. Had to put cotton balls in my ears to be able to sleep–was too tired to enjoy the city the next day. Rooms are TINY. I picked the room because it had two queen size beds–but the room barely had space to fit them. With family of four in the room it was tight. With all that said, rooms are clean and they’ve made an effort to update them. The hotel is in Marina district with lots of good places to eat, within walking distance to Presidio. May be good hotel for young stay-up-late adults on a budget
Selecione Executar e analise o sentimento juntamente com o nível de confiança. Dê uma olhada no texto e compare-o com a análise de sentimento que o serviço retornou.

Neste exercício você usou o Language Studio para criar um novo recurso de idioma ou usar um recurso de idioma existente. Você habilitou o recurso em Configurações antes de experimentar o serviço de mineração de sentimento e opinião. Em seguida, você testou o serviço com três trechos de texto.

Limpar
Se não pretende fazer mais exercícios, exclua todos os recursos que não precisa mais. Isso evita acumular custos desnecessários.

Abra o portal do Azure e selecione o grupo de recursos que contém o recurso que você criou. Selecione o recurso e selecione Excluir e depois Sim para confirmar. O recurso é então excluído.

Instruções de uso dos laboratórios extraídas e traduzidas para pt-BR dos seguintes links:

https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html

https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html
