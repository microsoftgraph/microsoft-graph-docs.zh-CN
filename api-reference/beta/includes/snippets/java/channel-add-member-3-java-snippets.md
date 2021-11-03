---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d19d240e9f66fd26183f21799f01193708b4ca34
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689140"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
conversationMember.roles = rolesList;
conversationMember.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users('jacob@contoso.com')"));

graphClient.teams("ece6f0a1-7ca4-498b-be79-edf6c8fc4d82").channels("19:56eb04e133944cf69e603c5dac2d292e@thread.skype").members()
    .buildRequest()
    .post(conversationMember);

```