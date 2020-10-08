---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e87823b25858d32a03a9b2b256d6f0f23ed8c57
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373453"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = new Channel();
channel.membershipType = ChannelMembershipType.PRIVATE;
channel.displayName = "My First Private Channel";
channel.description = "This is my first private channels";
LinkedList<ConversationMember> membersList = new LinkedList<ConversationMember>();
AadUserConversationMember members = new AadUserConversationMember();
members.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/users('{user_id}')"));
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
members.roles = rolesList;
membersList.add(members);
channel.members = membersList;

graphClient.teams("{group_id}").channels()
    .buildRequest()
    .post(channel);

```