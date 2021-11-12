---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c786be5b2c6c9fdac7614f1f12681a86e741285768bad804a2414dfd7bab78cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328788"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
event.originalStartTimeZone = "originalStartTimeZone-value";
event.originalEndTimeZone = "originalEndTimeZone-value";
ResponseStatus responseStatus = new ResponseStatus();
responseStatus.response = ResponseType.NONE;
responseStatus.time = OffsetDateTimeSerializer.deserialize("2016-10-19T10:37:00Z");
event.responseStatus = responseStatus;
event.recurrence = null;
event.uid = "iCalUId-value";
event.reminderMinutesBeforeStart = 99;
event.isOnlineMeeting = true;
event.onlineMeetingProvider = OnlineMeetingProviderType.TEAMS_FOR_BUSINESS;
event.isReminderOn = true;
event.hideAttendees = false;
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Red category");
event.categories = categoriesList;

graphClient.me().events("{id}")
    .buildRequest()
    .patch(event);

```