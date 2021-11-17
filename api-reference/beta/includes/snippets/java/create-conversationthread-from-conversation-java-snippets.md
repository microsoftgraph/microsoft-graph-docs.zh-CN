---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fff38f47533a13efd547d353bbaa7b9b4a528a52
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60987127"
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

graphClient.groups("4d81ce71-486c-41e9-afc5-e41bf2d0722a").conversations("AAQkAGRhZmRhMWM3LTYwZTktNDZmYy1hNWU1LThhZWU4NzI2YTEyZgAQABKPPJ682apIiV1UFlj7XxY=").threads()
    .buildRequest()
    .post(conversationThread);

```