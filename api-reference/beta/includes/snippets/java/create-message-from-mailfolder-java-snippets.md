---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ef7e2d32698fb2a9c46ba6067d85c6ebd57671b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979199"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.receivedDateTime = CalendarSerializer.deserialize("2016-10-19T10:37:00Z");
message.sentDateTime = CalendarSerializer.deserialize("2016-10-19T10:37:00Z");
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