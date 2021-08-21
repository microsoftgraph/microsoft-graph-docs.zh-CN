---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98a93fba8501bad52f631f0ef522daa4a0fd03c4d4205218f565409320c1b361
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220498"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String reason = "reason-value";

String duration = "duration-value";

String ticketNumber = "ticketNumber-value";

String ticketSystem = "ticketSystem-value";

graphClient.privilegedRoles("{id}")
    .selfActivate(PrivilegedRoleSelfActivateParameterSet
        .newBuilder()
        .withReason(reason)
        .withDuration(duration)
        .withTicketNumber(ticketNumber)
        .withTicketSystem(ticketSystem)
        .build())
    .buildRequest()
    .post();

```