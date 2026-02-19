# SDC_project
'틈만나면' 팀의 통계 데이터 대회 프로젝트 공간입니다 : )


<html>
<body>
<!--StartFragment--><h2 class="text-text-100 mt-3 -mb-1 text-[1.125rem] font-bold">프로젝트 개요</h2>
<p class="font-claude-response-body break-words whitespace-normal leading-[1.7]">전세사기 피해가 월 1,000건 이상 지속되는 상황에서, 서울시 전세 거래 데이터 기반으로 <strong>이상거래를 탐지</strong>하고 <strong>고위험 지역을 사전에 식별</strong>하는 분석 체계를 구축했습니다.</p>
<div class="overflow-x-auto w-full px-2 mb-6">
구분 | 내용
-- | --
데이터 | 국토교통부 실거래가 데이터 (2023.6 ~ 2024.12)
규모 | 전세 약 169,779건 + 매매 약 169,779건, 주택유형 4종
기술 스택 | Python (pandas, numpy, scikit-learn, matplotlib, seaborn)
담당 역할 | Z-score 이상거래 탐지 로직 설계 및 행정동 단위 위험도 분석

</div>
<hr class="border-border-200 border-t-0.5 my-3 mx-1.5">
<h2 class="text-text-100 mt-3 -mb-1 text-[1.125rem] font-bold">정책 제안</h2>
<ol class="[li_&amp;]:mb-0 [li_&amp;]:mt-1 [li_&amp;]:gap-1 [&amp;:not(:last-child)_ul]:pb-1 [&amp;:not(:last-child)_ol]:pb-1 list-decimal flex flex-col gap-1 pl-8 mb-3">
<li class="whitespace-normal break-words pl-2"><strong>고위험 지역 제도적 지정</strong>: 클러스터 1 해당 행정동을 '집중관리구역'으로 지정, 자치구 조례를 통한 법적 근거 마련</li>
<li class="whitespace-normal break-words pl-2"><strong>시민 대상 전세 리스크 정보 제공</strong>: 리스크 지도 데이터를 공공·민간 부동산 플랫폼과 연동, 데이터 기반 경향성 안내에 초점</li>
<li class="whitespace-normal break-words pl-2"><strong>상시 조기경보 체계</strong>: 동별 이상 스코어 정기 업데이트, 리스크 급증 지역 사전경고 지정</li>
</ol>
<hr class="border-border-200 border-t-0.5 my-3 mx-1.5">
<h2 class="text-text-100 mt-3 -mb-1 text-[1.125rem] font-bold">분석 한계 및 향후 과제</h2>
<ul class="[li_&amp;]:mb-0 [li_&amp;]:mt-1 [li_&amp;]:gap-1 [&amp;:not(:last-child)_ul]:pb-1 [&amp;:not(:last-child)_ol]:pb-1 list-disc flex flex-col gap-1 pl-8 mb-3">
<li class="whitespace-normal break-words pl-2">비아파트 통합(오피스텔+연립다세대+단독다가구)으로 매칭 실패율을 낮췄으나, 유형별 매매가 차이로 인한 전세가율 왜곡 가능성 존재</li>
<li class="whitespace-normal break-words pl-2">상위 위험 자치구 내 행정동만 분석하여, 저위험 자치구 내 개별 고위험 행정동은 누락될 수 있음</li>
<li class="whitespace-normal break-words pl-2">위험지표 간 상관이 높을 수 있어(Z3+ ↔ 상위 10% 등), 종합위험지수에 중복 반영 가능성 있음</li>
<li class="whitespace-normal break-words pl-2">향후 PCA 적용 후 클러스터링, 전체 행정동 대상 분석 확장, 시계열 기반 조기경보 로직 추가 검토 필요</li>
</ul>
<hr class="border-border-200 border-t-0.5 my-3 mx-1.5">
<h2 class="text-text-100 mt-3 -mb-1 text-[1.125rem] font-bold">담당 역할</h2>
<ul class="[li_&amp;]:mb-0 [li_&amp;]:mt-1 [li_&amp;]:gap-1 [&amp;:not(:last-child)_ul]:pb-1 [&amp;:not(:last-child)_ol]:pb-1 list-disc flex flex-col gap-1 pl-8 mb-3">
<li class="whitespace-normal break-words pl-2">조건조합 반복 실험을 통한 <strong>전세가율 산출 로직 최적화</strong></li>
<li class="whitespace-normal break-words pl-2">Z-score 기반 <strong>이상거래 탐지 로직 설계</strong> 및 4개 위험지표 정의</li>
<li class="whitespace-normal break-words pl-2">자치구 → 행정동 <strong>2단계 위험도 분석 프레임워크</strong> 구축</li>
<li class="whitespace-normal break-words pl-2">KMeans 클러스터링을 통한 <strong>4개 리스크 유형</strong> 도출 및 클러스터별 대응 전략 제안</li></ul><!--EndFragment-->
</body>
</html>
