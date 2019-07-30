---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 889d1faf5d328255fea7e0404c0ea39829cf9951
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933816"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<InvitationParticipantInfo> targetsList = new LinkedList<InvitationParticipantInfo>();
InvitationParticipantInfo targets = new InvitationParticipantInfo();
targets.endpointType = EndpointType.DEFAULT;
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "550fae72-d251-43ec-868c-373732c2704f";
user.tenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47";
user.displayName = "Heidi Steen";
identity.user = user;
targets.identity = identity;
targets.languageId = "en-US";
targets.region = "westus";

targetsList.add(targets);

CallDisposition targetDisposition = CallDisposition.DEFAULT;

int timeout = 99;

boolean maskCallee = False;

boolean maskCaller = False;

graphClient.app().calls("{id}")
    .redirect(targetsList,targetDisposition,timeout,maskCallee,maskCaller,callbackUri)
    .buildRequest()
    .post();

```