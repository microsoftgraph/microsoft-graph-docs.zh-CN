---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1a588d530c5828b312e8c02ac468123cb4e089c0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877306"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

OutlookTask outlookTask = new OutlookTask();
outlookTask.subject = "Shop for children's weekend";
DateTimeTimeZone startDateTime = new DateTimeTimeZone();
startDateTime.dateTime = "2016-05-03T09:00:00";
startDateTime.timeZone = "Eastern Standard Time";
outlookTask.startDateTime = startDateTime;
DateTimeTimeZone dueDateTime = new DateTimeTimeZone();
dueDateTime.dateTime = "2016-05-05T16:00:00";
dueDateTime.timeZone = "Eastern Standard Time";
outlookTask.dueDateTime = dueDateTime;

graphClient.me().outlook().tasks()
    .buildRequest( requestOptions )
    .post(outlookTask);

```