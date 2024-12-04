<h1>🎥 Recomendador de Filmes com Base em Similaridade de Usuários - MovieLens 100k</h1>
    <p>Este projeto utiliza o dataset <strong>MovieLens 100k</strong> para construir um sistema de recomendação de filmes baseado na similaridade de cosseno entre usuários. 
    A aplicação identifica os filmes que um usuário pode gostar, utilizando o método de <strong>k-vizinhos mais próximos (KNN)</strong> e a matriz usuário-item.</p>
    <h2>📁 Dataset</h2>
    <p>O dataset utilizado neste projeto é o <strong>MovieLens 100k</strong>, que contém 100.000 avaliações de 943 usuários sobre 1.682 filmes.</p>
    <ul>
        <li><strong>Fonte do dataset:</strong> MovieLens 100k</li>
        <li><strong>Formato do arquivo:</strong> u.data</li>
    </ul>
    <h3>📊 Estrutura do Dataset</h3>
    <ul>
        <li><strong>user_id:</strong> ID do usuário que avaliou o filme.</li>
        <li><strong>movie_id:</strong> ID do filme avaliado.</li>
        <li><strong>rating:</strong> Nota atribuída pelo usuário (entre 1 e 5).</li>
        <li><strong>timestamp:</strong> Momento em que a avaliação foi realizada (removido para simplificação do projeto).</li>
    </ul>
    <h2>🚀 Funcionalidades</h2>
    <ol>
        <li><strong>Matriz Usuário-Item:</strong> Criação de uma matriz onde as linhas representam usuários e as colunas representam filmes. Cada célula contém a avaliação dada por um usuário a um filme, com valores 0 para itens não avaliados.</li>
        <li><strong>Cálculo da Similaridade de Cosseno:</strong> Mede a similaridade entre os vetores de avaliações de usuários para identificar os vizinhos mais próximos.</li>
        <li><strong>k-Vizinhos Mais Próximos:</strong> Identifica os <code>k</code> usuários mais similares ao usuário-alvo.</li>
        <li><strong>Predição de Notas:</strong> Calcula a nota esperada para filmes não avaliados pelo usuário-alvo, utilizando as avaliações dos vizinhos mais próximos e suas similaridades.</li>
        <li><strong>Recomendação de Filmes:</strong> Retorna os 10 filmes mais bem classificados (com as maiores notas previstas) para o usuário-alvo.</li>
    </ol>
