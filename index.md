<p align="center">
  <img src="/assets/images/logo.png" alt="COALab Logo" width="220">
</p>

<div class="coalab-hero" style="
  background: linear-gradient(135deg, #004b8d 0%, #006bb3 40%, #00a0b3 100%);
  color: white;
  padding: 2.5rem 1.5rem;
  border-radius: 12px;
  margin-bottom: 2rem;
  text-align: center;
">
  <h1 style="margin-top:0; margin-bottom:0.5rem;">
    Cognition, Oral & Written Language Disorders, and AI Laboratory (COALab)
  </h1>
  <p style="max-width: 720px; margin:0 auto; font-size:1.05rem;">
    AI-driven research on speech, language, reading, and learning across development.
  </p>
</div>

<!-- Language toggle buttons -->
<div class="lang-toggle">
  <button type="button" data-lang="en" class="active">English</button>
  <button type="button" data-lang="fr">Français</button>
</div>

<!-- ENGLISH CONTENT -->
<div class="lang lang-en">

## Welcome

The Cognition, Oral & Written Language Disorders, and AI Laboratory (COALab) integrates speech-language pathology, developmental neuroscience, and artificial intelligence to advance research, assessment, and intervention supporting children with communication and learning disorders.

---

## Research Highlights

- **Voice-AI for early risk detection of neurodevelopmental disorders** – Developing automated speech- and language-based machine learning tools to identify early markers of communication, cognitive, and socio-emotional vulnerabilities in children before clinical challenges fully emerge.

- **Neural foundations of language and executive function development in developmental language disorder** – Using fNIRS and behavioral methods to investigate how neural systems supporting language, working memory, and cognitive control develop in children with and without DLD, including in bilingual contexts.

- **Personalized speech-language therapy using reinforcement learning** – Designing adaptive decision-support systems that recommend individualized intervention targets and therapy sequences to optimize learning outcomes over time.

- **Computational models of dyslexia** – Building and testing computational and statistical models to understand the linguistic, cognitive, and perceptual mechanisms underlying developmental dyslexia, including cross-linguistic influences.

---

## Quick Links

<div class="cta-buttons">
  <a href="{{ '/people/' | relative_url }}">People / Équipe</a>
  <a href="{{ '/publications/' | relative_url }}">Publications</a>
  <a href="{{ '/opportunities/' | relative_url }}">Join COALab / Rejoindre le COALab</a>
</div>

---

## Latest News

For more, see the [News / Nouvelles]({{ '/news/' | relative_url }}) page.

- Month Year – Short news item (e.g., new grant, paper, or invited talk).
- Month Year – Another news item.

</div> <!-- end .lang-en -->

<!-- FRENCH CONTENT -->
<div class="lang lang-fr">

## Bienvenue

Le Laboratoire sur la cognition, les troubles du langage oral et écrit et l’IA (COALab) intègre l’orthophonie, la neuroscience du développement et l’intelligence artificielle afin de faire progresser la recherche, l’évaluation et l’intervention auprès des enfants ayant des difficultés de communication et d’apprentissage.

---

## Faits saillants de la recherche

- **IA vocale pour la détection précoce des troubles neurodéveloppementaux** – Développer des outils automatisés basés sur la parole et le langage afin d’identifier les premiers marqueurs de vulnérabilités communicationnelles, cognitives et socioémotionnelles chez l’enfant, avant l’apparition de difficultés cliniques manifestes.

- **Fondements neuronaux du développement du langage et des fonctions exécutives dans le trouble développemental du langage** – Utiliser la spectroscopie fonctionnelle dans le proche infrarouge (fNIRS) et des mesures comportementales pour étudier comment les systèmes neuronaux soutenant le langage, la mémoire de travail et le contrôle cognitif se développent chez les enfants avec et sans TDL, y compris en contexte bilingue.

- **Orthophonie personnalisée à l’aide de l’apprentissage par renforcement** – Concevoir des systèmes d’aide à la décision adaptatifs qui recommandent des cibles d’intervention individualisées et des séquences thérapeutiques optimales au fil du temps.

- **Modèles computationnels de la dyslexie** – Élaborer et tester des modèles computationnels et statistiques afin de mieux comprendre les mécanismes linguistiques, cognitifs et perceptuels sous-jacents à la dyslexie développementale, notamment dans une perspective translinguistique.

---

## Liens rapides

<div class="cta-buttons">
  <a href="{{ '/people/' | relative_url }}">Équipe / People</a>
  <a href="{{ '/publications/' | relative_url }}">Publications</a>
  <a href="{{ '/opportunities/' | relative_url }}">Rejoindre le COALab / Join COALab</a>
</div>

---

## Dernières nouvelles

Pour plus de détails, consultez la page [News / Nouvelles]({{ '/news/' | relative_url }}).

- Mois Année – Brève nouvelle (p. ex. nouvelle subvention, article ou présentation invitée).
- Mois Année – Autre nouvelle importante.

</div> <!-- end .lang-fr -->

<!-- Language toggle script -->
<script>
document.addEventListener('DOMContentLoaded', function() {
  function setLang(lang) {
    document.querySelectorAll('.lang').forEach(function(el) {
      el.style.display = el.classList.contains('lang-' + lang) ? 'block' : 'none';
    });

    document.querySelectorAll('.lang-toggle button').forEach(function(btn) {
      btn.classList.toggle('active', btn.dataset.lang === lang);
    });
  }

  var buttons = document.querySelectorAll('.lang-toggle button');
  buttons.forEach(function(btn) {
    btn.addEventListener('click', function() {
      setLang(btn.dataset.lang);
    });
  });

  // Default language: English
  setLang('en');
});
</script>

