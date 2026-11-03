<!-- ---
title: "Design and Construction of a Bow-Tie and Superlattices"
collection: publication
category: project_reports
permalink: /publication/mit-visiting-report
date: 2025-12-01
venue: 'Visiting Research Student Report - MIT'
paperurl: 'https://drive.google.com/file/d/1jt8FfUzbLkf77rd4wqaEOnbNeljl-ykx/preview'
citation: '<b>Hrishikesh Malladi</b>. (2025). &quot;Design and Construction of a Bow-Tie and Superlattices.&quot;'
---

Independently designed and bench-tested a Bow-Tie Lattice and superlattice setup for future Quantum-Gas Microscope upgrades in the BEC V lab.

<iframe src="https://drive.google.com/file/d/1jt8FfUzbLkf77rd4wqaEOnbNeljl-ykx/preview" width="640" height="480"></iframe> -->


---
title: "Design and Construction of a Bow-Tie and Superlattices"
collection: publication
category: project_reports
permalink: /publication/mit-visiting-report
date: 2025-12-01
venue: 'Visiting Research Student Report - MIT'
paperurl: 'https://drive.google.com/file/d/1jt8FfUzbLkf77rd4wqaEOnbNeljl-ykx/preview'
citation: '<b>Hrishikesh Malladi</b>. (2025). &quot;Design and Construction of a Bow-Tie and Superlattices.&quot;'
---

Independently designed and bench-tested a Bow-Tie Lattice and superlattice setup for future Quantum-Gas Microscope upgrades in the BEC V lab.

<!-- Interactive Slide Deck Viewer -->
<div class="slide-deck-container" style="max-width: 100%; margin: 20px auto; text-align: center; background: #f9f9f9; padding: 20px; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
  
  <!-- Slide Image Display -->
  <div style="position: relative; width: 100%; overflow: hidden;">
    <img id="slideImage" src="{{ base_path }}/images/bow-tie-lattice-slides/Bow_tie_Lattice (1)_1.png" alt="Presentation Slide" style="width: 100%; height: auto; border: 1px solid #ddd; border-radius: 4px;">
  </div>

  <!-- Navigation Controls -->
  <div style="margin-top: 15px; display: flex; justify-content: center; align-items: center; gap: 15px;">
    <button onclick="prevSlide()" style="padding: 8px 16px; cursor: pointer; background: #333; color: #fff; border: none; border-radius: 4px; font-weight: bold;">&#10094; Prev</button>
    <span id="slideCounter" style="font-family: monospace; font-size: 1em; color: #333;">Slide 1 / X</span>
    <button onclick="nextSlide()" style="padding: 8px 16px; cursor: pointer; background: #333; color: #fff; border: none; border-radius: 4px; font-weight: bold;">Next &#10095;</button>
  </div>

</div>

<script>
  const slides = [
    "{{ base_path }}/images/bow-tie-lattice-slides/Bow_tie_Lattice (1)_1.png",
    "{{ base_path }}/images/bow-tie-lattice-slides/Bow_tie_Lattice (1)_2.png",
    "{{ base_path }}/images/bow-tie-lattice-slides/Bow_tie_Lattice (1)_3.png",
    "{{ base_path }}/images/bow-tie-lattice-slides/Bow_tie_Lattice (1)_4.png",
    "{{ base_path }}/images/bow-tie-lattice-slides/Bow_tie_Lattice (1)_5.png"
  ];

  let currentIndex = 0;
  const slideImage = document.getElementById("slideImage");
  const slideCounter = document.getElementById("slideCounter");

  function updateSlide() {
    slideImage.src = slides[currentIndex];
    slideCounter.innerText = `Slide ${currentIndex + 1} / ${slides.length}`;
  }

  function nextSlide() {
    if (currentIndex < slides.length - 1) {
      currentIndex++;
      updateSlide();
    }
  }

  function prevSlide() {
    if (currentIndex > 0) {
      currentIndex--;
      updateSlide();
    }
  }

  document.addEventListener("DOMContentLoaded", function() {
    slideCounter.innerText = `Slide 1 / ${slides.length}`;
  });

  document.addEventListener('keydown', function(event) {
    if (event.key === 'ArrowRight') {
      nextSlide();
    } else if (event.key === 'ArrowLeft') {
      prevSlide();
    }
  });
</script>