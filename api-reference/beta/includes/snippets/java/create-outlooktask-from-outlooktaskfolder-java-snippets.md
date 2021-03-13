---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa762ab6aa87998f5bc2f4e4474be57c33249a4a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774318"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTask outlookTask = new OutlookTask();
outlookTask.subject = "Shop for dinner";
DateTimeTimeZone startDateTime = new DateTimeTimeZone();
startDateTime.dateTime = "2016-04-23T18:00:00";
startDateTime.timeZone = "Pacific Standard Time";
outlookTask.startDateTime = startDateTime;
DateTimeTimeZone dueDateTime = new DateTimeTimeZone();
dueDateTime.dateTime = "2016-04-25T13:00:00";
dueDateTime.timeZone = "Pacific Standard Time";
outlookTask.dueDateTime = dueDateTime;

graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPXAAA=").tasks()
    .buildRequest()
    .post(outlookTask);

```