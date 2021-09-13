---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae3cd8dcc84ff9ce2770cac891de0ac3b98124236b25ae6f0d273c0c1456e897
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277259"
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