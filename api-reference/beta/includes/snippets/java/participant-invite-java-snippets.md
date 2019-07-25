---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b09feb49453bcb8039c5d4675577c87f150b702a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877070"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<InvitationParticipantInfo> participantsList = new LinkedList<InvitationParticipantInfo>();
InvitationParticipantInfo participants = new InvitationParticipantInfo();
participants.endpointType = EndpointType.DEFAULT;
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "550fae72-d251-43ec-868c-373732c2704f";
user.tenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47";
user.displayName = "Heidi Steen";
identity.user = user;
participants.identity = identity;
participants.languageId = "languageId-value";
participants.region = "region-value";
participants.replacesCallId = "replacesCallId-value";

participantsList.add(participants);

String clientContext = "clientContext-value";

graphClient.app().calls("{id}").participants()
    .invite(participantsList,clientContext)
    .buildRequest()
    .post();

```