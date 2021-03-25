---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ab88080eef06e4bb37bbbcc5959d834de581716
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208575"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Call call = new Call();
call.callbackUri = "https://bot.contoso.com/callback";
LinkedList<InvitationParticipantInfo> targetsList = new LinkedList<InvitationParticipantInfo>();
InvitationParticipantInfo targets = new InvitationParticipantInfo();
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.displayName = "John";
user.id = "112f7296-5fa4-42ca-bae8-6a692b15d4b8";
identity.user = user;
targets.identity = identity;
targetsList.add(targets);
call.targets = targetsList;
LinkedList<Modality> requestedModalitiesList = new LinkedList<Modality>();
requestedModalitiesList.add(Modality.AUDIO);
call.requestedModalities = requestedModalitiesList;
ServiceHostedMediaConfig mediaConfig = new ServiceHostedMediaConfig();
call.mediaConfig = mediaConfig;

graphClient.communications().calls()
    .buildRequest()
    .post(call);

```