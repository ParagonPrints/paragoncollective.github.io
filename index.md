---
layout: default
title: Paragon Collective - Coming Soon!
---

<div class="announcement">
  <h1>ParaBox Coming Fall 2025</h1>
  <p>Get ready for ParaBox, our innovative at-home STEAM kit designed to spark curiosity and learning through engaging, hands-on activities delivered right to your doorstep. Each kit will explore exciting scientific and artistic concepts, perfect for learners of all ages.</p>

  <h2>Help Us Design the Perfect Experience!</h2>
  <p>We're working hard to create the best possible ParaBox experience. Your feedback is invaluable!</p>

  <div class="survey-call-to-action">
    <label for="language-select">Choose your preferred language:</label>
    <select id="language-select">
      <option value="en">English</option>
      <option value="ar">العربية</option>
      <option value="fr">Français</option>
      </select>
    <button id="survey-button">Go to Survey</button>
  </div>
</div>

<script>
  const surveyButton = document.getElementById('survey-button');
  const languageSelect = document.getElementById('language-select');

  surveyButton.addEventListener('click', () => {
    const selectedLanguage = languageSelect.value;
    let surveyURL = '';

    switch (selectedLanguage) {
      case 'en':
        surveyURL = 'https://tally.so/r/3jEq8J';
        break;
      case 'ar':
        surveyURL = 'https://tally.so/r/w7jbXL';
        break;
      case 'fr':
        surveyURL = 'https://tally.so/r/wzgNE1';
        break;
      default:
        surveyURL = 'https://tally.so/r/3jEq8J';
    }

    if (surveyURL) {
      window.location.href = surveyURL;
    } else {
      alert('Please select a language.');
    }
  });
</script>