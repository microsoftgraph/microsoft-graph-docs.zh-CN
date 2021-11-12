---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f591a57e90fe88a7658885d3acc1546ecf3b8f6f3d0c1419eb3512bf97c9202b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221326"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.receivedDateTime = OffsetDateTimeSerializer.deserialize("2016-10-19T10:37:00Z");
message.sentDateTime = OffsetDateTimeSerializer.deserialize("2016-10-19T10:37:00Z");
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