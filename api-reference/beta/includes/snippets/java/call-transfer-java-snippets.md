---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fa840a8b66589ebd2f818da5418da5e23e08c1f7
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933810"
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
    .transfer(transferTarget)
    .buildRequest()
    .post();

```