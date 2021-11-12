---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37e3e299ab257cbb12d820baeecefa51bf2da5c2dc1e7afc5ebba0dbcbd58ac6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104011"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "content-value";
post.body = body;

graphClient.groups("{id}").threads("{id}")
    .reply(ConversationThreadReplyParameterSet
        .newBuilder()
        .withPost(post)
        .build())
    .buildRequest()
    .post();

```