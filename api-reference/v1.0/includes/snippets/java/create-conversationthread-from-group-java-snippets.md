---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87db74012f90b8b6ea72e7aa145b34fb699e4c209b799af9a908ab3ebcd0d3c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904317"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThread conversationThread = new ConversationThread();
conversationThread.topic = "New Conversation Thread Topic";
LinkedList<Post> postsList = new LinkedList<Post>();
Post posts = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "this is body content";
posts.body = body;
LinkedList<Recipient> newParticipantsList = new LinkedList<Recipient>();
Recipient newParticipants = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "Alex Darrow";
emailAddress.address = "alexd@contoso.com";
newParticipants.emailAddress = emailAddress;
newParticipantsList.add(newParticipants);
posts.newParticipants = newParticipantsList;
postsList.add(posts);
PostCollectionResponse postCollectionResponse = new PostCollectionResponse();
postCollectionResponse.value = postsList;
PostCollectionPage postCollectionPage = new PostCollectionPage(postCollectionResponse, null);
conversationThread.posts = postCollectionPage;

graphClient.groups("{id}").threads()
    .buildRequest()
    .post(conversationThread);

```