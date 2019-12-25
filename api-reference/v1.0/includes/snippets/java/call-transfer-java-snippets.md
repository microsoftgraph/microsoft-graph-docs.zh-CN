---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c773ac9e48febda2ce4c973b80efe206b6d3718
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865830"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InvitationParticipantInfo transferTarget = new InvitationParticipantInfo();
transferTarget.endpointType = "default";
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "550fae72-d251-43ec-868c-373732c2704f";
user.displayName = "Heidi Steen";
identity.user = user;
transferTarget.identity = identity;
transferTarget.replacesCallId = "replacesCallId-value";

String clientContext = "9e90d1c1-f61e-43e7-9f75-d420159aae08";

graphClient.communications().calls("{id}")
    .transfer(transferTarget)
    .buildRequest()
    .post();

```