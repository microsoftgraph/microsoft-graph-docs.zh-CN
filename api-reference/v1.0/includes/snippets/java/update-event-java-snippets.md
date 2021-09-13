---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c2c9091ddacc7d3ea543615fc629723fd0959498360d0038a0eeaae38506d44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277890"
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
event.recurrence = null;
event.iCalUId = "iCalUId-value";
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