---
title: "Generation of Rubidium Atom Cloud in a MOT and Magnetic Transport Optimization"
collection: publication
category: project_reports
permalink: /publication/nthu-visiting-report
date: 2024-07-01
venue: 'Visiting Research Student Report - National Tsing Hua University'
paperurl: 'https://drive.google.com/file/d/11ERnjmbX6S44J4exHxktn64weSe8KRBs/preview'
citation: '<b>Hrishikesh Malladi</b>. (2024). &quot;Generation of Rubidium Atom Cloud in a MOT and Magnetic Transport Optimization.&quot;'
---

Worked on a BEC experiment, consistently generating an Rb MOT and optimizing atom transfer to the optical dipole trap (ODT), achieving a 60% transfer rate.

<!-- Interactive Slide Deck Viewer -->
<div class="slide-deck-container" style="max-width: 100%; margin: 20px auto; text-align: center; background: #f9f9f9; padding: 20px; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
  
  <!-- Slide Image Display -->
  <div style="position: relative; width: 100%; overflow: hidden;">
    <img id="slideImage" src="{{ base_path }}/images/nthu_slides/2024_Summer_Project_Report (1)_1" alt="Presentation Slide" style="width: 100%; height: auto; border: 1px solid #ddd; border-radius: 4px;">
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
    "{{ base_path }}/images/nthu_slides/2024_Summer_Project_Report (1)_1",
    "{{ base_path }}/images/nthu_slides/2024_Summer_Project_Report (1)_2",
    "{{ base_path }}/images/nthu_slides/2024_Summer_Project_Report (1)_3",
    "{{ base_path }}/images/nthu_slides/2024_Summer_Project_Report (1)_4",
    "{{ base_path }}/images/nthu_slides/2024_Summer_Project_Report (1)_5"
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

**MOT Expansion Dynamics: Before vs. After Optimization**

<div style="display: flex; flex-wrap: wrap; justify-content: space-between; gap: 20px; margin-top: 15px;">
    <div style="flex: 1; min-width: 300px; text-align: center;">
        <span style="font-weight: bold; display: block; margin-bottom: 10px;">Before Optimization</span>
        <iframe src="{{ base_path }}/images/MOT_Expansion/MOT Expansion Videos/MOT_33ms_3.41mm_CMP(2.679A,2.233A,0.305A)_2024-07-19T16-51-03.105.avi" width="100%" height="280" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen style="border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);"></iframe>
    </div>
    <div style="flex: 1; min-width: 300px; text-align: center;">
        <span style="font-weight: bold; display: block; margin-bottom: 10px;">After Optimization</span>
        <iframe src="{{ base_path }}/images/MOT_Expansion/MOT Expansion Videos/MOT_33ms_2.82mm_CMP(1.96A,2.15A,0.1A)_2024-07-19T16-12-57.493.avi" width="100%" height="280" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen style="border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);"></iframe>
    </div>
</div>