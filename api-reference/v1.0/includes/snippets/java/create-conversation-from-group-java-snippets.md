---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef23596f14c0159178f3ba5a73d4f3031e984323
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889576"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Conversation conversation = new Conversation();
conversation.topic = "New locations for this quarter";
LinkedList<ConversationThread> threadsList = new LinkedList<ConversationThread>();
ConversationThread threads = new ConversationThread();
LinkedList<Post> postsList = new LinkedList<Post>();
Post posts = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "What do we know so far?";
posts.body = body;
LinkedList<Recipient> newParticipantsList = new LinkedList<Recipient>();
Recipient newParticipants = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "Adele Vance";
emailAddress.address = "AdeleV@contoso.onmicrosoft.com";
newParticipants.emailAddress = emailAddress;
newParticipantsList.add(newParticipants);
posts.newParticipants = newParticipantsList;
postsList.add(posts);
threads.posts = postsList;
threadsList.add(threads);
conversation.threads = threadsList;

graphClient.groups("29981b6a-0e57-42dc-94c9-cd24f5306196").conversations()
    .buildRequest()
    .post(conversation);

```