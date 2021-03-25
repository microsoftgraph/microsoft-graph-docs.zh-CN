---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b28814bc8df27abe7db3986f1bea7dda716b87a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208999"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String memberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33";

graphClient.groups("{id}")
    .evaluateDynamicMembership(GroupEvaluateDynamicMembershipParameterSet
        .newBuilder()
        .withMemberId(memberId)
        .build())
    .buildRequest()
    .post();

```