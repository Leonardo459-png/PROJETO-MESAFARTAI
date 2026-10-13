
ESCOPO GERAL DO PROJETO & REQUISITOS TÉCNICOS

O ecossistema do MESAFARTAI é composto por 4 grandes pilares tecnológicos desenvolvidos 100% em Python:

1.	Interface Conversacional (Front-End - Streamlit):
o	Chat interativo para cadastro de doações e consultas de ONGs.
o	Alternância de perfil na barra lateral ([Sou Doador | Sou ONG]).

2.	Motor de NLU & Trava de Segurança (Back-End - Scikit-Learn / Spacy):
o	Classificação de intenções (cadastrar_doacao, solicitar_alimentos, consultar_status, fora_de_escopo).
o	Mecanismo de Threshold (ex: < 0.60) com resposta de Fallback amigável quando a frase for ambígua.

3.	Extração de Entidades (Regex):
o	Captura automática de quantidades (kg, caixas, unidades), tipos de alimentos e prazos de validade (hoje, amanhã, 18h).

3.	Matchmaking Logístico & Banco de Dados (KNN + SQLite3):
o	Algoritmo KNN para calcular o match perfeito entre a oferta do doador e a ONG receptora mais próxima.
o	Banco de dados SQLite3 para persistência de doadores, receptores, doações e histórico de coletas.

Script de Banco de Dados (src/database.py)
Criar o script Python responsável por inicializar o banco de dados relacional SQLite3 (mesafartai.db) com as tabelas fundamentais e popular com dados de teste.


Prompt Utilizado:

Gerar Ícone de logotipo 3D isométrico moderno para um sistema inteligente de doação de alimentos chamado 'MESAFARTAI- MESAFARTAI – Logística e Inteligência Assistiva no Combate à Fome'. O ícone apresenta uma caixa de entregas ou prato estilizado integrado a nós de rede digital e um símbolo de pino de localização, representando logística inteligente e conexão por IA. Cores vibrantes: verde esmeralda, laranja quente e azul ciano. Renderização 3D limpa, textura fosca suave, sombras suaves, isolado em um fundo branco sólido.
