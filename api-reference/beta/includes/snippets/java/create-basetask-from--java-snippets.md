---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95c1bf5813e3550f6b8783906b829dc089b7eb7f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130106"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BaseTask baseTask = new BaseTask();
ItemBody body = new ItemBody();
baseTask.body = body;
baseTask.bodyLastModifiedDateTime = OffsetDateTimeSerializer.deserialize("String (timestamp)");
baseTask.completedDateTime = OffsetDateTimeSerializer.deserialize("String (timestamp)");
DateTimeTimeZone dueDateTime = new DateTimeTimeZone();
baseTask.dueDateTime = dueDateTime;
DateTimeTimeZone startDateTime = new DateTimeTimeZone();
baseTask.startDateTime = startDateTime;
baseTask.importance = Importance.LOW;
PatternedRecurrence recurrence = new PatternedRecurrence();
baseTask.recurrence = recurrence;
baseTask.displayName = "String";
baseTask.status = TaskStatus_v2.NOT_STARTED;
PersonalTaskProperties personalProperties = new PersonalTaskProperties();
baseTask.personalProperties = personalProperties;

graphClient.me().tasks().lists("AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNi").tasks()
    .buildRequest()
    .post(baseTask);

```