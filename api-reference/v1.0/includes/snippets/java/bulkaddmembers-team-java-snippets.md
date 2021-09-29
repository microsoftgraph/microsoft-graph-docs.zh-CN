---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78a7f5e8211faa1fed2ae0da0bf3f877a18b9e0f
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996732"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<ConversationMember> valuesList = new LinkedList<ConversationMember>();
AadUserConversationMember values = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
values.roles = rolesList;
values.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"));

valuesList.add(values);
AadUserConversationMember values1 = new AadUserConversationMember();
LinkedList<String> rolesList1 = new LinkedList<String>();
rolesList1.add("owner");
values1.roles = rolesList1;
values1.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"));

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