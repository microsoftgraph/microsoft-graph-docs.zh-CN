---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6606d257fabdbad7dc169edf36c502bac06422f7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965320"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String memberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33";

String membershipRule = "(user.displayName -startsWith "EndTestUser")";

graphClient.groups()
    .evaluateDynamicMembership(memberId,membershipRule)
    .buildRequest()
    .post();

```