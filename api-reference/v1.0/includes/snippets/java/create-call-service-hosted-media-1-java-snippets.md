---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9109d0440fe3a1643e28d263a1bc3270355472b3cc346ff7077efd8063b84e43
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221035"
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