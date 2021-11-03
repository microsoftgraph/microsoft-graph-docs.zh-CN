---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3aad0b204d84a8c56794bcb3b2394e711e7c16f9
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696545"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
conversationMember.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/users/jacob@contoso.com"));
conversationMember.visibleHistoryStartDateTime = OffsetDateTimeSerializer.deserialize("2019-04-18T23:51:43.255Z");
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
conversationMember.roles = rolesList;

graphClient.chats("19:cf66807577b149cca1b7af0c32eec122@thread.v2").members()
    .buildRequest()
    .post(conversationMember);

```