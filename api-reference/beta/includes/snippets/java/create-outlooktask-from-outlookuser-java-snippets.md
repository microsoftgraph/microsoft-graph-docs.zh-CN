---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42961691122845f0a1211f9f0df19720671b320bef25d2d2aa58e5bb3e384656
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163659"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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