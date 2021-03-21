---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32e01686948f2144371a7b1962cd53f8debeb65e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978918"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String reason = "reason-value";

String ticketNumber = "ticketNumber-value";

String ticketSystem = "ticketSystem-value";

graphClient.privilegedRoleAssignments("{id}")
    .makePermanent(PrivilegedRoleAssignmentMakePermanentParameterSet
        .newBuilder()
        .withReason(reason)
        .withTicketNumber(ticketNumber)
        .withTicketSystem(ticketSystem)
        .build())
    .buildRequest()
    .post();

```