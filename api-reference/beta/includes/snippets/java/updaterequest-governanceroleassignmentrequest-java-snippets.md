---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a635fccd080b9b05110e44177c9ea15646be95855265b6f081ad145a73d0bdd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219754"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedAccess("azureResources").roleAssignmentRequests("7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee")
    .updateRequest(GovernanceRoleAssignmentRequestUpdateRequestParameterSet
        .newBuilder()
        .withDecision(null)
        .withAssignmentState(null)
        .withSchedule(null)
        .withReason(null)
        .build())
    .buildRequest()
    .post();

```