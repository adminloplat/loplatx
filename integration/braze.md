---
description: loplat X와 braze dashboard 연동하기
---

# braze 연동하기

{% embed url="https://youtu.be/sBNmHW8Ll6o" %}

1. **loplat X** 계정과 **braze 계정**이 생성되어야 합니다.
2. 각 dashboard 연결을 위해선, Rest API 만들어야 합니다.
   * braze rest API 필수 권한 요소
     * users.track&#x20;
     * campaigns.trigger.send&#x20;
     * campaigns.list&#x20;
     * canvas.trigger.send&#x20;
     * canvas.list
3. API를 만들었다면, loplat X API 관리에 braze rest API를 추가 해주세요
4. 권한이 모두 확인되면 API는 정상적으로 연결됩니다.

모든 연동이 완료되었다면, 캠페인 연동을 사용할 수 있습니다.&#x20;

{% content-ref url="../campaigns/create/campaign-intergration.md" %}
[campaign-intergration.md](../campaigns/create/campaign-intergration.md)
{% endcontent-ref %}

이제 캠페인 연동을 통해 자유롭게 캠페인을 진행하세요.&#x20;
