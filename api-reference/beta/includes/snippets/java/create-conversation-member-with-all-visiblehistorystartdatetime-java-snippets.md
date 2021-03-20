---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23eb84808f9eb2252cdac5ea0cf75654235baf38
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
conversationMember.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"));
conversationMember.visibleHistoryStartDateTime = OffsetDateTimeSerializer.deserialize("0001-01-01T00:00:00Z");

graphClient.chats("19:cf66807577b149cca1b7af0c32eec122@thread.v2").members()
    .buildRequest()
    .post(conversationMember);

```