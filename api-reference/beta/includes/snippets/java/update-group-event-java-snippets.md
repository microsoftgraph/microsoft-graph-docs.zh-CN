---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15105016675914b20f85c8f7a0f8b738179d95154cab9783a7fa8666c122faee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161444"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
event.originalStartTimeZone = "originalStartTimeZone-value";
event.originalEndTimeZone = "originalEndTimeZone-value";
ResponseStatus responseStatus = new ResponseStatus();
responseStatus.response = ResponseType.NONE;
responseStatus.time = OffsetDateTimeSerializer.deserialize("datetime-value");
event.responseStatus = responseStatus;
event.uid = "iCalUId-value";
event.reminderMinutesBeforeStart = 99;
event.isReminderOn = true;

graphClient.groups("{id}").events("{id}")
    .buildRequest()
    .patch(event);

```