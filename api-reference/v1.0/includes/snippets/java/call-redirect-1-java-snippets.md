---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 306a915a9575d174083cb08192a7996a13ed546f946988437606e63c4c34b84c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278619"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<InvitationParticipantInfo> targetsList = new LinkedList<InvitationParticipantInfo>();
InvitationParticipantInfo targets = new InvitationParticipantInfo();
IdentitySet identity = new IdentitySet();
Identity application = new Identity();
application.displayName = "test bot 2";
application.id = "22bfd41f-550e-477d-8789-f6f7bd2a5e8b";
identity.application = application;
targets.identity = identity;

targetsList.add(targets);

String callbackUri = "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039";

graphClient.communications().calls("491f0b00-ffff-4bc9-a43e-b226498ec22a")
    .redirect(CallRedirectParameterSet
        .newBuilder()
        .withTargets(targetsList)
        .withTimeout(null)
        .withCallbackUri(callbackUri)
        .build())
    .buildRequest()
    .post();

```