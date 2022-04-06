---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fddbb779af820c23b58c8325d62e42ea960dfeed
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528102"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Task baseTask = new Task();
baseTask.textBody = "String";
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
TaskViewpoint viewpoint = new TaskViewpoint();
baseTask.viewpoint = viewpoint;

graphClient.me().tasks().lists("AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt").tasks("AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT")
    .buildRequest()
    .patch(baseTask);

```