---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e625a0caa80eb6e41a4f2e2b490ba83c8f286d0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976085"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> participantsList = new LinkedList<String>();
participantsList.add("");

String clientContext = "clientContext-value";

graphClient.communications().calls("{id}").participants()
    .muteAll(ParticipantMuteAllParameterSet
        .newBuilder()
        .withParticipants(participantsList)
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```