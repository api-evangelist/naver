---
title: "VictoriaMetrics 운영기 2편 — 장비 증설 없이 리소스 위기를 해결한 3단계 최적화 전략"
url: "https://d2.naver.com/helloworld/5788040"
date: "2026-07-21"
feed_url: "https://d2.naver.com/d2.atom"
---
VictoriaMetrics 운영기 1편 에서는 네이버 검색의 대규모 메트릭 저장소 VictoriaMetrics 클러스터의 규모, 2계층 아키텍처, 180대 노드의 무중단 장비 교체와 증설 전략을 소개했습니다. 2편에서는 장비를 더 늘리지 않고 리소스 위기를 해결하기 위해 진행한 소프트웨어적 최적화 과정을 다룹니다. 메모리 문제를 해결한 뒤에도 쿠버네티스 전환은 계속 빨라졌고, 컨테이너 수는 수백만 개를 넘어섰습니다.
