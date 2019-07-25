---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9c138fdf788aa64698b6e3fb55ff7eb8bd8a9583
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864603"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InvitationParticipantInfo transferTarget = new InvitationParticipantInfo();
transferTarget.endpointType = EndpointType.DEFAULT;
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "550fae72-d251-43ec-868c-373732c2704f";
user.tenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47";
user.displayName = "Heidi Steen";
identity.user = user;
transferTarget.identity = identity;
transferTarget.languageId = "languageId-value";
transferTarget.region = "region-value";
transferTarget.replacesCallId = "replacesCallId-value";

String clientContext = "clientContext-value";

graphClient.app().calls("{id}")
    .transfer(transferTarget,target,replacesCallId)
    .buildRequest()
    .post();

```