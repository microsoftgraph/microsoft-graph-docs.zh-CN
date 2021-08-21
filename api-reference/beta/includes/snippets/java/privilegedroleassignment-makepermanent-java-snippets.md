---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a44919399287765a553e5140ca3d7e45d762c3a40d8a547be124bb40e8b1be7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328749"
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