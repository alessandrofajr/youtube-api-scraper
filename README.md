# YouTube API Scraper
 Esse repositório contém o código necessário para utilizar a API do YouTube para coletar dados de canais, entre eles: nome do canal, título de cada vídeo publicado, o ID de cada vídeo, a data da publicação do conteúdo, a data de extração dos dados, o número de likes, o número de dislikes, o número de visualizações, o número de comentários e a URL das thumbnails dos vídeos. Há ainda um script para comparar dois datasets e verificar se o vídeo foi removido utilizando a biblioteca Pandas (ver arquivo "compare-data.ipynb").

## Fonte dos dados

Os dados são obtidos por meio da API do YouTube. Veja como obter a sua chave da API na documentação oficial do [Google](https://developers.google.com/youtube/v3/getting-started?hl=pt_br)

## Dados resultados

O script oferece os dados em CSV ao final. Neste repositório há:

- `canal_insper.csv` contém dados do canal do Insper
- `alessandro.csv` contém dados do meu canal pessoal
- `alessandro.csv` contém dados do meu canal pessoal após tornar um vídeo privado

#### Dicionário

| variable             | definition                                                                         | 
| -------------------- | ---------------------------------------------------------------------------------- | 
| channel              | Nome do canal                                                                      |
| title                | Título do vídeo                                                                    |
| video_id             | ID do vídeo (pode ser adicionado ao final da URL https://www.youtube.com/watch?v=) |
| video_description    | Descrição do vídeo                                                                 |
| published_date       | Data da publicação do vídeo                                                        |
| extraction_date      | Data da extração dos dados                                                         |
| likes                | Número de likes                                                                    |
| dislikes             | Número de dislikes                                                                 |
| views                | Número de visualizações                                                            |
| comment              | Número de comentários                                                              |
| thumbnail            | Link da thumbnail do vídeo                                                         |
| merge                | "left_only" indica quando um dado foi removido do dataset                          |
