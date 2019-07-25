---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 17cfcc578a93f75dea68af7d1c9379e3d502d1a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879921"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.receivedDateTime = "2016-10-19T10:37:00Z";
message.sentDateTime = "2016-10-19T10:37:00Z";
message.hasAttachments = true;
message.subject = "subject-value";
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "content-value";
message.body = body;
message.bodyPreview = "bodyPreview-value";

graphClient.me().mailFolders("{id}").messages()
    .buildRequest()
    .post(message);

```