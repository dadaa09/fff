```
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Flashcards MC Hariel</title>
<style>
  :root {
    --primary-color: #3a86ff;
    --secondary-color: #264653;
    --accent-color: #f4a261;
    --background-color: #f0f4f8;
    --card-background: #ffffff;
    --font-family: 'Poppins', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    --shadow-color: rgba(58, 134, 255, 0.2);
  }

  * {
    box-sizing: border-box;
  }

  body {
    margin: 0;
    background-color: var(--background-color);
    font-family: var(--font-family);
    color: var(--secondary-color);
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    line-height: 1.5;
  }

  header {
    background: linear-gradient(135deg, var(--primary-color), var(--accent-color));
    color: white;
    padding: 2.25rem 1.5rem;
    text-align: center;
    box-shadow: 0 4px 12px var(--shadow-color);
  }

  header h1 {
    margin: 0;
    font-weight: 700;
    font-size: 2.75rem;
    letter-spacing: 1.1px;
  }

  header p {
    margin-top: 0.5rem;
    font-size: 1.2rem;
    font-weight: 500;
    font-style: italic;
  }

  main {
    flex-grow: 1;
    max-width: 1000px;
    margin: 2.5rem auto 3.5rem;
    padding: 0 1.25rem;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 2rem;
  }

  .flashcard {
    background-color: var(--card-background);
    border-radius: 14px;
    box-shadow: 0 12px 20px rgba(0,0,0,0.08);
    cursor: pointer;
    perspective: 1200px;
    transition: transform 0.35s ease, box-shadow 0.3s ease;
    position: relative;
    outline-offset: 4px;
  }

  .flashcard:hover {
    box-shadow: 0 16px 30px rgba(0, 0, 0, 0.15);
  }

  .flashcard:focus {
    outline: 3px solid var(--primary-color);
  }

  .flashcard-inner {
    position: relative;
    width: 100%;
    height: 240px;
    text-align: center;
    transition: transform 0.7s cubic-bezier(0.4, 0, 0.2, 1);
    transform-style: preserve-3d;
    border-radius: 14px;
  }

  .flashcard.flipped .flashcard-inner {
    transform: rotateY(180deg);
  }

  .flashcard-front,
  .flashcard-back {
    position: absolute;
    width: 100%;
    height: 240px;
    backface-visibility: hidden;
    border-radius: 14px;
    padding: 2rem 1.8rem;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 1.3rem;
    font-weight: 600;
    color: var(--secondary-color);
    user-select: none;
  }

  .flashcard-front {
    background: linear-gradient(135deg, #a8dadc, #457b9d);
    box-shadow: inset 0 6px 16px rgba(255 255 255 / 0.75);
    color: white;
  }

  .flashcard-back {
    background: linear-gradient(135deg, #ffe5d9, #f4a261);
    color: #264653;
    font-weight: 500;
    transform: rotateY(180deg);
  }

  footer {
    text-align: center;
    padding: 1.2rem 1rem;
    font-size: 1rem;
    color: #555;
    font-weight: 500;
    border-top: 1px solid #ddd;
  }

  /* Responsive text sizes */
  @media (max-width: 480px) {
    header h1 {
      font-size: 2rem;
    }
    header p {
      font-size: 1rem;
    }
    .flashcard-front, .flashcard-back {
      font-size: 1.1rem;
      padding: 1.5rem 1.2rem;
      height: 200px;
    }
    main {
      gap: 1.3rem;
      grid-template-columns: 1fr;
      max-width: 90vw;
      margin: 2rem auto 2rem;
      padding: 0 1rem;
    }
  }
</style>
</head>
<body>
<header>
  <h1>Flashcards MC Hariel</h1>
  <p>Conheça fatos e curiosidades sobre o MC Hariel</p>
</header>
<main id="flashcards-container">
  <div class="flashcard" tabindex="0" role="button" aria-pressed="false" aria-label="Flashcard sobre nome verdadeiro do MC Hariel">
    <div class="flashcard-inner">
      <div class="flashcard-front">Qual é o nome verdadeiro do MC Hariel?</div>
      <div class="flashcard-back">Hariel Lucas da Silva</div>
    </div>
  </div>
  <div class="flashcard" tabindex="0" role="button" aria-pressed="false" aria-label="Flashcard sobre a carreira do MC Hariel">
    <div class="flashcard-inner">
      <div class="flashcard-front">Qual é a principal carreira do MC Hariel?</div>
      <div class="flashcard-back">Cantor e compositor de funk</div>
    </div>
  </div>
  <div class="flashcard" tabindex="0" role="button" aria-pressed="false" aria-label="Flashcard sobre a origem do MC Hariel">
    <div class="flashcard-inner">
      <div class="flashcard-front">De onde é o MC Hariel?</div>
      <div class="flashcard-back">São Paulo, Brasil</div>
    </div>
  </div>
  <div class="flashcard" tabindex="0" role="button" aria-pressed="false" aria-label="Flashcard sobre as músicas do MC Hariel">
    <div class="flashcard-inner">
      <div class="flashcard-front">Quais são algumas músicas populares do MC Hariel?</div>
      <div class="flashcard-back">"Acorda", "Coração de Pedra", "Coração de Aço"</div>
    </div>
  </div>
  <div class="flashcard" tabindex="0" role="button" aria-pressed="false" aria-label="Flashcard sobre o estilo musical do MC Hariel">
    <div class="flashcard-inner">
      <div class="flashcard-front">Qual é o estilo musical do MC Hariel?</div>
      <div class="flashcard-back">Funk e rap</div>
    </div>
  </div>
  <div class="flashcard" tabindex="0" role="button" aria-pressed="false" aria-label="Flashcard sobre a mensagem nas músicas do MC Hariel">
    <div class="flashcard-inner">
      <div class="flashcard-front">Qual é a mensagem comum nas músicas do MC Hariel?</div>
      <div class="flashcard-back">Superação e vivências da vida nas comunidades</div>
    </div>
  </div>
  <div class="flashcard" tabindex="0" role="button" aria-pressed="false" aria-label="Flashcard sobre a popularidade do MC Hariel">
    <div class="flashcard-inner">
      <div class="flashcard-front">Como é a popularidade do MC Hariel?</div>
      <div class="flashcard-back">Ele é muito popular entre os jovens e nas redes sociais.</div>
    </div>
  </div>
</main>
<footer>
  Desenvolvido com ❤️ para destacar o talento do MC Hariel
</footer>
<script>
  document.querySelectorAll('.flashcard').forEach(card => {
    card.addEventListener('click', () => {
      card.classList.toggle('flipped');
      const isPressed = card.getAttribute('aria-pressed') === 'true';
      card.setAttribute('aria-pressed', !isPressed);
    });
    card.addEventListener('keydown', e => {
      if(e.key === 'Enter' || e.key === ' ') {
        e.preventDefault();
        card.click();
      }
    });
  });
</script>
</body>
</html>
```
