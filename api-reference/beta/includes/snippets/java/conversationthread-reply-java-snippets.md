---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e59869ee0f864e23b31432480167551711856027
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862889"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "content-value";
post.body = body;

graphClient.groups("{id}").threads("{id}")
    .reply(post)
    .buildRequest()
    .post();

```