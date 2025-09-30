## Testes no Cloud Azure

Este repositório documenta os testes realizados com a Análise de Sentimento utilizando o serviço de IA do Azure. O objetivo foi configurar recursos Azure, criar um ambiente de Machine Learning e rodar uma análise demonstrativa, validando os principais conceitos e etapas de uso prático da IA na plataforma.
Conceitos Fundamentais do Azure Utilizados

    Azure AI Foundry e Cognitive Services: Utilizados para provisionar recursos prontos para consumo de modelos de IA, como análise de texto e sentimentos em diversas línguas, via APIs e interface gráfica.

    Workspace do Azure Machine Learning: Ambiente colaborativo na nuvem para gerenciar experimentos, datasets, modelos e endpoints de inferência. Cada workspace serve como ponto central para o ciclo de vida de projetos de Machine Learning.

    Gestão de Recursos e Permissões: Organização e controle do acesso aos recursos de AI por meio de grupos de recursos, controle de assinaturas e definição de modelos de precificação.

    Painel de Resultados: Disponibilização de métricas detalhadas sobre o sentimento do texto analisado, incluindo confiança e classificação (positivo, neutro, negativo).

Processo de Teste e Resultados
1. Criação do Projeto no Azure AI Foundry

    Um recurso textspeech-resource foi criado, sob a assinatura "Pago pelo Uso" na camada Standard S0.

    A configuração inicial envolveu gerenciamento de acesso, associação de recursos, e exibição do painel de gestão (ver imagem "Criacao_Projeto.jpg").

2. Configuração do Workspace no Azure ML

    Criado um novo workspace chamado aulaAzureSpeech para centralizar experimentos e recursos de Machine Learning.

    Seleção da assinatura, criação de grupo de recursos e escolha da região. Configuração conforme melhores práticas para isolar ambientes de teste (ver imagem "Criacao_Estudio.jpg").

3. Execução e Validação da Análise de Sentimento

    Teste realizado na interface gráfica do Azure (Cognitive Services) usando a frase:

        “Hoje o dia está bonito e parece que não irá chover!”

    Resultado fornecido pelo serviço:

        Sentimento detectado: Positivo

        Confiança: 97% positivo, 3% neutro, 0% negativo

        O modelo segmenta e avalia a confiança frase a frase, utilizando processamento de linguagem natural (ver imagem "Resultado.jpg").

Conclusão Técnica

    O fluxo demonstrado mostra como provisionar recursos, configurar workspaces e consumir modelos pré-treinados na nuvem Azure.

    O serviço de Análise de Sentimento do Azure mostrou-se eficaz para avaliações rápidas de texto em português, indicando potencial para aplicações de atendimento, análise de redes sociais e automação de relatórios.

    Todos os passos são replicáveis via portal web, facilitando integração contínua e experimentação em projetos de IA.
