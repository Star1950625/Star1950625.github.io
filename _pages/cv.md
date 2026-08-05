---
layout: cv
permalink: /cv/
title: CV
nav: true
nav_order: 5
cv_format: rendercv # options: rendercv, jsonresume
description: >
  Curriculum Vitae of Shunxiang Liao.
toc:
  sidebar: left
---

<style>
  /* Bootstrap grid missing from al-folio v1 Tailwind compat — restore the
     two-column CV layout (date column + content column) manually. */
  .cv .row {
    display: flex;
    flex-wrap: wrap;
  }
  .cv .date-column {
    flex: 0 0 25%;
    max-width: 25%;
    text-align: center;
  }
  .cv .col-xs-10,
  .cv .col-sm-10,
  .cv .col-md-10 {
    flex: 0 0 75%;
    max-width: 75%;
    padding-left: 8px;
  }
  @media (max-width: 767px) {
    .cv .date-column,
    .cv .col-xs-10,
    .cv .col-sm-10,
    .cv .col-md-10 {
      flex: 0 0 100%;
      max-width: 100%;
      text-align: left;
    }
  }
  /* Give the CV cards a bit of breathing room */
  .cv .card {
    border: 1px solid var(--global-divider-color);
    border-radius: 0.25rem;
  }
  .cv .mt-3 {
    margin-top: 1rem;
  }
  .cv .p-3 {
    padding: 1rem;
  }
  .cv .location {
    margin-top: 0.5rem;
    margin-bottom: 0;
  }
</style>
