---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 167246919b9847d81da1fa71f6f039ab1960636c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979473"
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