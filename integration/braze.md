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
