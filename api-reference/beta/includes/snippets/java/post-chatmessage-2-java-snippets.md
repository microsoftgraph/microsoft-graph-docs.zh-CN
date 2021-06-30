---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e86399962c3448e5e3f4bf55645eabd679802fb6
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208002"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "Hello World <at id=\"0\">Jane Smith</at>";
chatMessage.body = body;
LinkedList<ChatMessageMention> mentionsList = new LinkedList<ChatMessageMention>();
ChatMessageMention mentions = new ChatMessageMention();
mentions.id = 0;
mentions.mentionText = "Jane Smith";
ChatMessageMentionedIdentitySet mentioned = new ChatMessageMentionedIdentitySet();
Identity user = new Identity();
user.displayName = "Jane Smith";
user.id = "ef1c916a-3135-4417-ba27-8eb7bd084193";
user.userIdentityType = TeamworkUserIdentityType.AAD_USER;
mentioned.user = user;
mentions.mentioned = mentioned;
mentionsList.add(mentions);
chatMessage.mentions = mentionsList;

graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels("19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2").messages()
    .buildRequest()
    .post(chatMessage);

```