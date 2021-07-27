---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e14314ae360db4063d49d312f686dca978d4436
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581379"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
conversationMember.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"));
conversationMember.visibleHistoryStartDateTime = OffsetDateTimeSerializer.deserialize("2019-04-18T23:51:43.255Z");
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
conversationMember.roles = rolesList;

graphClient.chats("19:cf66807577b149cca1b7af0c32eec122@thread.v2").members()
    .buildRequest()
    .post(conversationMember);

```