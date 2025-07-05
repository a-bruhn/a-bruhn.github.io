---
layout: post
title: Ultimate Attribution Error
date: 2025-07-05 11:11 +0200
categories: [concepts]
tags: [social psychology]
---

### Illustrative Diagram

<style>
  :root {
    --color-dispositional: rgba(135, 206, 250, 0.3);
    --color-dispositional-shadow: rgba(135, 206, 250, 0.6);

    --color-situational: rgba(72, 209, 204, 0.3);
    --color-situational-shadow: rgba(72, 209, 204, 0.6);
  }

  .uae-container {
    max-width: 600px;
    margin: 2em auto;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }

  .uae-table {
    display: grid;
    grid-template-columns: 110px 1fr 1fr;
    grid-template-rows: 45px 200px 200px;
    border-radius: 12px;
    overflow: hidden;
    user-select: none;
    background: transparent;
  }

  .uae-table > div {
    padding: 0;
    font-weight: 600;
    font-size: 1rem;
    text-align: center;
    background: transparent;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 1.5em;
  }

  .header-cell,
  .axis-label {
    font-weight: 700;
    font-size: 1.1rem;
    user-select: text;
    color: var(--text-light);
    transition: color 0.3s ease;
  }

  .quadrant {
    border: 2px solid transparent;
    border-radius: 10px;
    padding: 0;
    box-shadow: inset 0 0 20px;
    font-weight: 600;
  }

  .quadrant.dispositional {
    background-color: var(--color-dispositional);
    box-shadow: inset 0 0 20px var(--color-dispositional-shadow);
    color: var(--color-dispositional-text);
    border-color: var(--color-dispositional-text);
  }

  .quadrant.situational {
    background-color: var(--color-situational);
    box-shadow: inset 0 0 20px var(--color-situational-shadow);
    color: var(--color-situational-text);
    border-color: var(--color-situational-text);
  }

  .uae-table > div:not(.quadrant) {
    border: none;
  }

  .legend {
    margin-top: 1.5em;
    display: flex;
    gap: 2em;
    justify-content: flex-start;
    font-size: 1rem;
    color: var(--text-light);
    transition: color 0.3s ease;
  }

  .legend-item {
    display: flex;
    align-items: center;
    gap: 0.7em;
    user-select: none;
  }

  .legend-color {
    width: 24px;
    height: 24px;
    border-radius: 6px;
  }

  .legend-dispositional {
    background-color: var(--color-dispositional);
    box-shadow: 0 0 15px var(--color-dispositional-shadow);
    border: 2px solid var(--color-dispositional-text);
  }

  .legend-situational {
    background-color: var(--color-situational);
    box-shadow: 0 0 15px var(--color-situational-shadow);
    border: 2px solid var(--color-situational-text);
  }

  @media (prefers-color-scheme: dark) {
    .header-cell,
    .axis-label,
    .legend {
      color: var(--text-dark);
    }
  }
</style>

<div class="uae-container" role="region" aria-label="Ultimate Attribution Error quadrant chart">
  <div class="uae-table" aria-describedby="legend">
    
    <div></div>
    <div class="header-cell" tabindex="0">Ingroup</div>
    <div class="header-cell" tabindex="0">Outgroup</div>

    <div class="axis-label" tabindex="0">Positive Behavior</div>
    <div class="quadrant dispositional" tabindex="0">
      Our character:<br>typical for us
    </div>
    <div class="quadrant situational" tabindex="0">
      Exceptional case or external circumstances:<br>atypical for them
    </div>

    <div class="axis-label" tabindex="0">Negative Behavior</div>
    <div class="quadrant situational" tabindex="0">
      External circumstances:<br>atypical for us
    </div>
    <div class="quadrant dispositional" tabindex="0">
      Their character:<br>typical for them
    </div>
  </div>

  <div id="legend" class="legend" aria-label="Attribution legend">
    <div class="legend-item">
      <div class="legend-color legend-dispositional"></div>
      <span>Dispositional Attribution</span>
    </div>
    <div class="legend-item">
      <div class="legend-color legend-situational"></div>
      <span>Situational Attribution</span>
    </div>
  </div>
</div>
      
### Original Theory

**Pettigrew, T. F.** (1979). *The ultimate attribution error: Extending Allport's cognitive analysis of prejudice*. _Personality and Social Psychology Bulletin, 5_(4), 461–476. [https://doi.org/10.1177/014616727900500407](https://doi.org/10.1177/014616727900500407)
