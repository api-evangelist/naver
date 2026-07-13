---
title: "Inside VictoriaMetrics"
url: "https://d2.naver.com/helloworld/9290861"
date: "2026-06-08"
author: ""
feed_url: "https://d2.naver.com/d2.atom"
---
네이버 사내 기술 교류 행사인 NAVER ENGINEERING DAY 2026(5월)에서 발표되었던 세션을 공개합니다. 발표 내용 VictoriaMetrics의 수집(vmagent) → 라우팅(vminsert) → 저장(vmstorage) → 쿼리(vmselect) 순서로 내부 구조를 들여다기보고, 원리에 따라 수집의 좋은 구조를 살펴봅니다. 발표 대상 VictoriaMetrics 개발에 관심 있는 엔지니어 대규모 분산 시스템과 메트릭 인프라를 운영하는 엔지니어 목차 Architecture Overview vmagent: Scraping &amp; Remote Write vminsert: Ingestion Pipeline vmstorage: Data Storage vmselect: Query Executio
