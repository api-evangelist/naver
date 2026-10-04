---
title: "Hive는 잊으려 했지만, Spark는 기억하고 있었다: 사라진 get_table RPC 복원기"
url: "https://d2.naver.com/helloworld/7314597"
date: "2026-09-29"
feed_url: "https://d2.naver.com/d2.atom"
---
TApplicationException · UNKNOWN_METHOD Invalid method name: 'get_table' 이 글은 네이버의 Hadoop 플랫폼인 C3의 Metastore를 Apache Hive 4.2로 올리는 과정에서 Spark 잡(job)이 실패한 현상과 그 원인을 추적해, Metastore Thrift 인터페이스에서 조용히 사라졌던 RPC 하나를 복원하기까지의 과정을 다룹니다. 코드 변경 자체는 IDL 두 줄과 서버 구현 몇 줄이 전부지만, 그 이면에는 Thrift RPC의 동작 방식과 Hive와 Spark 사이의 오래된 버전 호환성이라는 맥락이 얽혀 있습니다. 그리고 직접 수정한 코드보다 훨씬 큰 비중을 차지하는 'Thrift 생성 코드를 어디까지 확인해야 변경이 완료되는가'라는 질문도 함께 다룹니다.
