---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa63436cc60b75f3358020bcd600fa50c3ab2e8d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209039"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String memberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33";

String membershipRule = "(user.displayName -startsWith "EndTestUser")";

graphClient.groups()
    .evaluateDynamicMembership(GroupEvaluateDynamicMembershipParameterSet
        .newBuilder()
        .withMemberId(memberId)
        .withMembershipRule(membershipRule)
        .build())
    .buildRequest()
    .post();

```