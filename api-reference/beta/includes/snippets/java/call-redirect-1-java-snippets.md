---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8cb3aee0460c6245f8ad05fb48e19c71b9870d8
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209893"
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
        .withTargetDisposition(null)
        .withTimeout(null)
        .withMaskCallee(null)
        .withMaskCaller(null)
        .withCallbackUri(callbackUri)
        .build())
    .buildRequest()
    .post();

```