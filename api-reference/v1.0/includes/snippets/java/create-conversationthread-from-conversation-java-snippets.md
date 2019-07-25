---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 454f54cf6cf046231cbb2aa161c30761cf7dd728
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883686"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThread conversationThread = new ConversationThread();
conversationThread.topic = "topic-value";
LinkedList<Post> postsList = new LinkedList<Post>();
Post posts = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "this is body content";
posts.body = body;
postsList.add(posts);
conversationThread.posts = postsList;

graphClient.groups("{id}").conversations("{id}").threads()
    .buildRequest()
    .post(conversationThread);

```