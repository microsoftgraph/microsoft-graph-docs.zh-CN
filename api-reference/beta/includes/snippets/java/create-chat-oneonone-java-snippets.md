---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78876ac59aa7a968bdd00c79dcfe611276a8fbaf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = new Chat();
chat.chatType = ChatType.ONE_ON_ONE;
LinkedList<ConversationMember> membersList = new LinkedList<ConversationMember>();
AadUserConversationMember members = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
members.roles = rolesList;
members.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"));
membersList.add(members);
AadUserConversationMember members1 = new AadUserConversationMember();
LinkedList<String> rolesList1 = new LinkedList<String>();
rolesList1.add("owner");
members1.roles = rolesList1;
members1.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"));
membersList.add(members1);
ConversationMemberCollectionResponse conversationMemberCollectionResponse = new ConversationMemberCollectionResponse();
conversationMemberCollectionResponse.value = membersList;
ConversationMemberCollectionPage conversationMemberCollectionPage = new ConversationMemberCollectionPage(conversationMemberCollectionResponse, null);
chat.members = conversationMemberCollectionPage;

graphClient.chats()
    .buildRequest()
    .post(chat);

```