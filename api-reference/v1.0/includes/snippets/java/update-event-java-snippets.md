---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 664bafb14155b14997bb1f8b1db82ad2cf02860b
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43770896"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
event.originalStartTimeZone = "originalStartTimeZone-value";
event.originalEndTimeZone = "originalEndTimeZone-value";
ResponseStatus responseStatus = new ResponseStatus();
responseStatus.response = ResponseType.NONE;
responseStatus.time = "datetime-value";
event.responseStatus = responseStatus;
event.recurrence = null;
event.iCalUId = "iCalUId-value";
event.reminderMinutesBeforeStart = 99;
event.isOnlineMeeting = true;
event.onlineMeetingProvider = OnlineMeetingProviderType.TEAMS_FOR_BUSINESS;
event.isReminderOn = true;

graphClient.me().events("{id}")
    .buildRequest()
    .patch(event);

```