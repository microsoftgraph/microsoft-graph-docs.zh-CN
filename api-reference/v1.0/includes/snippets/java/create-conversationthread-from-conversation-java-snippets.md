---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89f34b024d5616033c1dd9f765e796ec9db8c06b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068266"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThread conversationThread = new ConversationThread();
conversationThread.topic = "Take your wellness days and rest";
LinkedList<Post> postsList = new LinkedList<Post>();
Post posts = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "Waiting for the summer holidays.";
posts.body = body;
postsList.add(posts);
PostCollectionResponse postCollectionResponse = new PostCollectionResponse();
postCollectionResponse.value = postsList;
PostCollectionPage postCollectionPage = new PostCollectionPage(postCollectionResponse, null);
conversationThread.posts = postCollectionPage;

graphClient.groups("{id}").conversations("{id}").threads()
    .buildRequest()
    .post(conversationThread);

```