---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3fe7c7b6e84604ff738c5a3240016e9f154dad4d1779c96a78619a48b5cfe8f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902992"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
conversationMember.roles = rolesList;
conversationMember.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"));

graphClient.teams("{id}").channels("{id}").members()
    .buildRequest()
    .post(conversationMember);

```