---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6aa74f9f7b21887554cd85985304c1c6fee6a06
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979316"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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