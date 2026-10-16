---
title: "Python의 GC가 멀티프로세싱과 만나면 생기는 일 - Python과 Airflow, 그리고 관련된 문제 해결기 2편"
url: "https://d2.naver.com/helloworld/4149925"
date: "2026-10-08"
feed_url: "https://d2.naver.com/d2.atom"
---
Python의 멀티프로세싱과 Airflow의 task 동작 방식 - Python과 Airflow, 그리고 관련된 문제 해결기 1편 에서는 Airflow가 task를 실행할 때 요구되는 병렬성과 격리성을 살펴보고, 이를 만족하기 위해 Airflow가 task마다 만들었다 버리는 단기 프로세스와 만들어 두고 재사용하는 장기 프로세스를 모두 fork 방식으로 생성한다는 점을 확인했습니다. fork는 생성 속도와 메모리 효율 모두에서 spawn을 크게 앞섰지만, 두 가지 한계가 따라온다는 점도 언급했습니다. 부모의 자원을 그대로 승계한다는 점과, Python에서는 Copy-on-Write(COW)가 기대만큼 동작하지 않는다는 점입니다.
