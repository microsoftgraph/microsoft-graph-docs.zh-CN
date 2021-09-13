---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4120630482071408a5b5ae5816691fc56c745f510eb975a8b501523c5de1e1f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333830"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = new Channel();
channel.membershipType = ChannelMembershipType.PRIVATE;
channel.displayName = "My First Private Channel";
channel.description = "This is my first private channels";
LinkedList<ConversationMember> membersList = new LinkedList<ConversationMember>();
AadUserConversationMember members = new AadUserConversationMember();
members.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/users('62855810-484b-4823-9e01-60667f8b12ae')"));
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
members.roles = rolesList;
membersList.add(members);
ConversationMemberCollectionResponse conversationMemberCollectionResponse = new ConversationMemberCollectionResponse();
conversationMemberCollectionResponse.value = membersList;
ConversationMemberCollectionPage conversationMemberCollectionPage = new ConversationMemberCollectionPage(conversationMemberCollectionResponse, null);
channel.members = conversationMemberCollectionPage;

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5").channels()
    .buildRequest()
    .post(channel);

```