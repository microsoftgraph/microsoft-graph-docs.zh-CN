---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d508dacd96719bfd474ca94a98cf9bb7e831e32
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945132"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<InvitationParticipantInfo> participantsList = new LinkedList<InvitationParticipantInfo>();
InvitationParticipantInfo participants = new InvitationParticipantInfo();
participants.replacesCallId = "a7ebfb2d-871e-419c-87af-27290b22e8db";
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "278405a3-f568-4b3e-b684-009193463064";
user.displayName = "string";
identity.user = user;
participants.identity = identity;

participantsList.add(participants);

String clientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f";

graphClient.communications().calls("{id}").participants()
    .invite(participantsList,clientContext)
    .buildRequest()
    .post();

```