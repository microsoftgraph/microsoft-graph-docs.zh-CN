---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4936771367f281647cd0e67008a0e8f95c14b06e3bd1afa7e38f6999804e8d72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279494"
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