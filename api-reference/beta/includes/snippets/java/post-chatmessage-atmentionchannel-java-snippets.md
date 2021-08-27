---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fc4779bc84460c6f4bf4b513c6f023fd6afb7a415e74242f3eabfdc2843f2fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904268"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "<div><div><at id=\"0\">General</at>&nbsp;Hello there!</div></div>";
chatMessage.body = body;
LinkedList<ChatMessageMention> mentionsList = new LinkedList<ChatMessageMention>();
ChatMessageMention mentions = new ChatMessageMention();
mentions.id = 0;
mentions.mentionText = "General";
ChatMessageMentionedIdentitySet mentioned = new ChatMessageMentionedIdentitySet();
TeamworkConversationIdentity conversation = new TeamworkConversationIdentity();
conversation.id = "19:0b50940236084d258c97b21bd01917b0@thread.skype";
conversation.displayName = "General";
conversation.conversationIdentityType = TeamworkConversationIdentityType.CHANNEL;
mentioned.conversation = conversation;
mentions.mentioned = mentioned;
mentionsList.add(mentions);
chatMessage.mentions = mentionsList;

graphClient.teams("68a3e365-f7d9-4a56-b499-24332a9cc572").channels("19:0b50940236084d258c97b21bd01917b0@thread.skype").messages()
    .buildRequest()
    .post(chatMessage);

```