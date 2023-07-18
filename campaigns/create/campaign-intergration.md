---
description: 캠페인 생성 > 메시지 설정
---

# 캠페인 연동

Breze를 사용하기 위해선 먼저 loplat X와 시스템 연동이 필요합니다.&#x20;

{% content-ref url="../../integration/braze.md" %}
[braze.md](../../integration/braze.md)
{% endcontent-ref %}

위 **braze 페이지를 참고**하시고 연동 후 캠페인 연동을 사용하세요.

## 1. Braze dashboard -> loplat X(API-Triggered delivery 사용)

{% embed url="https://youtu.be/VsJcM9bdR70" %}

1. Braze dashboard 에서 새로운 Campaign 또는 canvas를 생성합니다.
   * **Campaign**
     * Schedule Delivery 에서 API-Triggered Delivery 선택
   * **Canvas**
     * Entry Schedule 에서 API-Triggered 선택
   * 이후 각 설정 및 생성을 완료 후 Campaign 또는 canvas ID를 복사합니다.
2. loplat X 이동 후 Campaign을 생성합니다.
   1. 설정 마지막 **캠페인 메시지 설정 > 메시지 알림 방식 선택 > braze 연동**을 선택 후 \
      **Trigger\[API-Triggered Delivery]** 선택합니다.
   2. braze에서 복사한 ID에 따라 Campaign 또는 Canvas를 선정해 줍니다.
   3. 마지막으로 하단에 **Braze Campaign ID** 또는 **Braze Canvas ID**를 입력하고 캠페인 생성을 완료합니다.

## 2. loplat X -> Braze dashboard(Custom event 사용)

{% embed url="https://youtu.be/ZCGUkCjSXRo" %}

1. loplat X에서 캠페인을 생성합니다.
   * 생성중 상위 모든 설정을 완료한 후 **braze 연동 > Add Custom Event 선택**
   * Event name 설정 후 하단 **Event name에 포함되어 Braze에 보내는 정보** 확인 후 캠페인 생성 완료
     * **Event name에 포함되어 Braze에 보내는 정보** (위치 설정값에 따라 보내지는 정보는 다를 수 있음)
       * 지오펜스 명
       * 지역조건: 광역시/도 단위
       * 지역조건: 시/구 단위
       * 지역조건: 동 단위
       * 브랜드명
       * 매장명
2. braze dashboard Campain 또는 Canvas에서 Custom Event 활용하기
   * **Campaign**
     1. Schedule Delivery 에서 Action-Based Delivery 선택
     2. Action-Based Scheduling Options>New Trigger Action에서 \
        Perform Custom Event 선택 후 Add Trigger
     3. 추가된 Perform Custom Event에서 loplat X campaign에서 \
        설정한 Event name을 찾아 설정을 완료
     4. 나머지 모든 설정 완료 후 Campaign 생성
   * **Canvas**
     1. Entry Schedule 에서 Action-Based 선택
     2. Action-Based Options>New Trigger Action에서\
        Perform Custom Event 선택 후 Add Trigger
     3. 추가된 Perform Custom Event에서 loplat X campaign에서 \
        설정한 Event name을 찾아 설정을 완료
     4. 나머지 모든 설정 완료 후 Canvas 생성
