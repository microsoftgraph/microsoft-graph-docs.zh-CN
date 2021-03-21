---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b78307251f3a0ec5bd6dd3acd8d8761dccbf22cb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978759"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
PostCollectionResponse postCollectionResponse = new PostCollectionResponse();
postCollectionResponse.value = postsList;
PostCollectionPage postCollectionPage = new PostCollectionPage(postCollectionResponse, null);
threads.posts = postCollectionPage;
threadsList.add(threads);
ConversationThreadCollectionResponse conversationThreadCollectionResponse = new ConversationThreadCollectionResponse();
conversationThreadCollectionResponse.value = threadsList;
ConversationThreadCollectionPage conversationThreadCollectionPage = new ConversationThreadCollectionPage(conversationThreadCollectionResponse, null);
conversation.threads = conversationThreadCollectionPage;

graphClient.groups("29981b6a-0e57-42dc-94c9-cd24f5306196").conversations()
    .buildRequest()
    .post(conversation);

```