---
title: "MLXP : Kubernetes LLM Serving  최적화 기술 도입기"
url: "https://d2.naver.com/helloworld/1059238"
date: "2026-06-11"
author: ""
feed_url: "https://d2.naver.com/d2.atom"
---
네이버 사내 기술 교류 행사인 NAVER ENGINEERING DAY 2026(5월)에서 발표되었던 세션을 공개합니다. 발표 내용 LLM 추론 성능을 극대화하기 위한 최신 기술들(KV Cache 인지 라우팅, Prefix Cache, 분산 멀티노드 서빙 등)을 Kubernetes 프로덕션 환경에 도입하는 과정에서 기존 인프라 스택(Istio 서비스 메시, 스케줄러, Pod 보호 정책)과 충돌하며 발생한 실전 문제들을 어떻게 진단하고 해결했는지 공유합니다. 발표 대상 Kubernetes 위에서 GPU 워크로드를 운영하는 플랫폼 엔지니어 LLM 서빙 인프라를 직접 구축·운영하는 MLOps / Infra 엔지니어 Istio 서비스 메시 환경에서 AI 워크로드를 다루는 DevOps 엔지니어 목차 배경 : MLXP와
