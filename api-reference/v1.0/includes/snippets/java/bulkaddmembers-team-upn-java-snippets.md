---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e9f1b572246f30ab3dd8ba84d5b2696883bda8d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688404"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<ConversationMember> valuesList = new LinkedList<ConversationMember>();
AadUserConversationMember values = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
values.roles = rolesList;
values.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"));

valuesList.add(values);
AadUserConversationMember values1 = new AadUserConversationMember();
LinkedList<String> rolesList1 = new LinkedList<String>();
rolesList1.add("owner");
values1.roles = rolesList1;
values1.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/users('alex@contoso.com')"));

valuesList.add(values1);
ConversationMemberCollectionResponse conversationMemberCollectionResponse = new ConversationMemberCollectionResponse();
conversationMemberCollectionResponse.value = valuesList;
ConversationMemberCollectionPage conversationMemberCollectionPage = new ConversationMemberCollectionPage(conversationMemberCollectionResponse, null);

graphClient.teams("e4183b04-c9a2-417c-bde4-70e3ee46a6dc").members()
    .add(ConversationMemberAddParameterSet
        .newBuilder()
        .withValues(valuesList)
        .build())
    .buildRequest()
    .post();

```