---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b00cb9cae5b4edc9d1f9c05060f50a4a502ff6c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981986"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String reason = "reason-value";

String ticketNumber = "ticketNumber-value";

String ticketSystem = "ticketSystem-value";

graphClient.privilegedRoleAssignments("{id}")
    .makePermanent(reason,ticketNumber,ticketSystem)
    .buildRequest()
    .post();

```