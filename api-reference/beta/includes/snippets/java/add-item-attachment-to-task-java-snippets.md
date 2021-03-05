---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccc8c4c77152c5723058c05fc1ebe6e1cdcbcaa6
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474753"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAttachment attachment = new ItemAttachment();
attachment.name = "Holiday event";
Event item = new Event();
item.subject = "Discuss gifts for children";
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "Let's look for funding!";
item.body = body;
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2020-01-12T18:00:00";
start.timeZone = "Pacific Standard Time";
item.start = start;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2020-01-12T19:00:00";
end.timeZone = "Pacific Standard Time";
item.end = end;
attachment.item = item;

graphClient.me().outlook().tasks("AAMkADAAAANXbdnAAA=").attachments()
    .buildRequest()
    .post(attachment);

```