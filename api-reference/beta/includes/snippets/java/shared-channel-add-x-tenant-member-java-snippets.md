---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fae23ac0231a0bf5f362f96eee17a0ec29567b28
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206842"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
conversationMember.roles = rolesList;
conversationMember.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users/bc3598dd-cce4-4742-ae15-173429951408"));
conversationMember.tenantId = "a18103d1-a6ef-4f66-ac64-e4ef42ea8681";

graphClient.teams("6a720ba5-7373-463b-bc9f-4cd04b5c6742").channels("19:LpxShHZZh9utjNcEmUS5aOEP9ASw85OUn05NcWYAhX81@thread.tacv2").members()
    .buildRequest()
    .post(conversationMember);

```