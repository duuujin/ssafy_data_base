# 팔로우 관계 구현하기
- 유저 <-> 유저 구조를 self 관계로 정의하고 symmetrical 속성을 False로 설정
- 프로필에서 팔로우 여부, 게시글, 댓글 정보 등을 효율적으로 조회 가능

# fixtures로 빠른 데이터 입출력 하기
- dumpdata와 loaddata를 통해 백업과 복원 작업을 수행할 수 있음
- 테스트 데이터나 초기 설정 데이터 관리가 쉬워짐

# 쿼리 최적화의 핵심
- select_related는 FK 관계를, prefetch_related는 N:M/역참조 관계를 최적화함
- annotate로 집계값을 추가하고, exists로 빠르게 존재 여부 확인 가능
