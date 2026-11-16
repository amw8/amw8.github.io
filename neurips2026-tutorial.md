---
layout: default
title: "Empirical Design in Reinforcement Learning for Physical AI · NeurIPS 2026 Tutorial"
permalink: /neurips2026-tutorial/
---

<p class="back-link"><a href="{{ '/' | relative_url }}">← Adam White</a></p>

<div class="tutorial-hero">
  <p class="tutorial-kicker">NeurIPS 2026 Tutorial · Sydney</p>
  <h1>Empirical Design in Reinforcement Learning for Physical AI</h1>
  <p class="tutorial-speakers"><a href="{{ '/' | relative_url }}">Adam White</a> · <a href="https://marthawhite.github.io/">Martha White</a> · <a href="https://andnp.github.io/">Andrew Patterson</a></p>
  <p class="tutorial-helpers">Hands-on sessions led by Andrew Patterson and Esraa Elelimy</p>
  <div class="profile-links">
    <span>Mon, Dec 7, 2026</span>
    <span>9:00 AM – 12:00 PM AEDT</span>
    <span>Grand BR B1</span>
  </div>
</div>

## Abstract

It is no secret that reinforcement learning algorithms are hard to apply in the real world, but why? The answer is not obvious, so we start with a concrete example: on a realistic industrial simulator, multiple widely used algorithms perform worse than a simple baseline. Attendees then dig into a hands-on session to find out why. Next, we step back and discuss what makes the real world hard. These challenges rarely show up in standard benchmarks, and our current algorithms were never designed for them. The rest of the tutorial is about bringing those concerns into the lab. We cover empirical methodology, new benchmarks, and the many ways researchers accidentally cheat. We also take a hard look at common bad practice in RL: too few random seeds, untuned baselines, and overconfident claims built on incorrect confidence intervals. A second hands-on session shows how easily these mistakes can mislead us about what will work in deployment. We do not offer a single checklist for running RL experiments. Instead, attendees leave with three key messages and practical tools they can use in their own work.

## Schedule

<table class="schedule-table">
<thead><tr><th>Time (AEDT)</th><th>Session</th><th>Presenter</th></tr></thead>
<tbody>
<tr><td>9:00 – 9:05</td><td><strong>Introduction and plan for the day.</strong> If you take three messages away today…</td><td>Adam</td></tr>
<tr><td>9:05 – 9:20</td><td><strong>Demonstration.</strong> Popular algorithms perform worse than a simple baseline on a realistic industrial simulator.</td><td>Adam</td></tr>
<tr class="row-handson"><td>9:20 – 9:40</td><td><strong>Hands-on session 1: You get one deployment.</strong> Get to the bottom of the failure. <a href="#hands-on-1">Details ↓</a></td><td>Andrew &amp; Esraa</td></tr>
<tr><td>9:40 – 10:05</td><td><strong>Challenges unique to the real world.</strong> What deployment demands that popular RL benchmarks do not, and why current algorithms are not designed for it.</td><td>Adam</td></tr>
<tr class="row-break"><td>10:05 – 10:30</td><td><strong>Break</strong></td><td></td></tr>
<tr><td>10:30 – 11:00</td><td><strong>Designing laboratory experiments aligned with real-world concerns.</strong> Empirical methodology, new benchmarks, common accidental cheating, and more.</td><td>Martha</td></tr>
<tr><td>11:00 – 11:15</td><td><strong>Common poor empirical practices in RL.</strong> Too few seeds, untuned baselines, and confidently incorrect claims (confidence intervals, distributions) that make us think our algorithms are ready for the real world.</td><td>Andrew</td></tr>
<tr class="row-handson"><td>11:15 – 11:40</td><td><strong>Hands-on session 2: Same agents, different conclusions.</strong> How these errors mislead us about what works in deployment. <a href="#hands-on-2">Details ↓</a></td><td>Andrew &amp; Esraa</td></tr>
<tr><td>11:40 – 11:50</td><td><strong>Wrap-up.</strong> If you take three messages away today…</td><td>Martha</td></tr>
</tbody>
</table>

## Hands-on Sessions

Both sessions run in Colab in your browser. Bring a laptop and a Google account; nothing needs to be installed.

<div class="handson-card" id="hands-on-1">
  <p class="handson-label">Hands-on session 1 · 20 minutes · Andrew &amp; Esraa</p>
  <h3>You get one deployment</h3>
  <p>You lead the ML team at a wastewater treatment plant, and the board has approved exactly one RL deployment. Your agent controls aeration: air costs money, but too little air lets ammonia through, and ammonia over the limit costs you your permit. You pick one algorithm and one learning rate, commit, and watch your agent run for years of plant time against a controller that never moves. Then we look at what it would have cost to find a better configuration on a real plant, and what happens to the best agent when the plant changes.</p>
  <div class="profile-links">
    <span class="link-pending">Colab notebook · coming soon</span>
  </div>
</div>

<div class="handson-card" id="hands-on-2">
  <p class="handson-label">Hands-on session 2 · 25 minutes · Andrew &amp; Esraa</p>
  <h3>Same agents, different conclusions</h3>
  <p>In the first session you ran the plant; now you write the paper. Nothing trains. You get the runs from the experiments in <a href="https://jmlr.org/papers/v25/23-0183.html">Empirical Design in Reinforcement Learning</a> and make the analysis choices yourself: how many seeds to report, which interval to trust, how to pick the best configuration from a sweep, and where to cut off an episode. Each common shortcut turns the same agents into a better-looking result. All of it runs on Mountain Car and PuddleWorld, on purpose: deployment-aligned evaluation is a protocol you can apply in any environment, not a reason to abandon simple problems.</p>
  <div class="profile-links">
    <span class="link-pending">Colab notebook · coming soon</span>
  </div>
</div>

## Resources

- Andrew Patterson, Samuel Neumann, Martha White, Adam White (2024). [Empirical Design in Reinforcement Learning](https://jmlr.org/papers/volume25/23-0183/23-0183.pdf). *Journal of Machine Learning Research*.
- Slides · coming soon
