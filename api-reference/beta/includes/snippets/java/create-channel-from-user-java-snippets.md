---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7c675de3720108a31b198eeb74ba68c98cb286f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959091"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = new Channel();
channel.membershipType = ChannelMembershipType.PRIVATE;
channel.displayName = "My First Private Channel";
channel.description = "This is my first private channels";
LinkedList<ConversationMember> membersList = new LinkedList<ConversationMember>();
AadUserConversationMember members = new AadUserConversationMember();
members.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users('{user_id}')"));
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
members.roles = rolesList;
membersList.add(members);
ConversationMemberCollectionResponse conversationMemberCollectionResponse = new ConversationMemberCollectionResponse();
conversationMemberCollectionResponse.value = membersList;
ConversationMemberCollectionPage conversationMemberCollectionPage = new ConversationMemberCollectionPage(conversationMemberCollectionResponse, null);
channel.members = conversationMemberCollectionPage;

graphClient.teams("{group_id}").channels()
    .buildRequest()
    .post(channel);

```