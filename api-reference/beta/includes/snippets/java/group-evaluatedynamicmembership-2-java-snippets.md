---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 917c60d673a3b72082fd550f3230ac4f2b179cf57c8f8cfb22910e572019d70f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333127"
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