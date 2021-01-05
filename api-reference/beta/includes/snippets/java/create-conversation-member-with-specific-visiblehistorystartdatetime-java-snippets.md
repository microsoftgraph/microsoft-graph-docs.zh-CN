---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d852bda2d3cf85d2104bed914cd012e8466215a9
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753220"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
conversationMember.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"));
conversationMember.visibleHistoryStartDateTime = "2019-04-18T23:51:43.255Z";

graphClient.chats("19:cf66807577b149cca1b7af0c32eec122@thread.v2").members()
    .buildRequest()
    .post(conversationMember);

```