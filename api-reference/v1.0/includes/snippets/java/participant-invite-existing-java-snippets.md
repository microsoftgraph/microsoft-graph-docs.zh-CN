---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b3b296d31513d77ac8426120e26461a5040421059ad09d64eee3d0a05cda7fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104320"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<InvitationParticipantInfo> participantsList = new LinkedList<InvitationParticipantInfo>();
InvitationParticipantInfo participants = new InvitationParticipantInfo();
participants.replacesCallId = "a7ebfb2d-871e-419c-87af-27290b22e8db";
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "7e1b4346-85a6-4bdd-abe3-d11c5d420efe";
user.displayName = "string";
identity.user = user;
participants.identity = identity;

participantsList.add(participants);

String clientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f";

graphClient.communications().calls("ab6233a5-20b7-4c5e-bea2-ce56c9776429").participants()
    .invite(ParticipantInviteParameterSet
        .newBuilder()
        .withParticipants(participantsList)
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```