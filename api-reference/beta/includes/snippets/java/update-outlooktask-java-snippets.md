---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b67c86f6bc83bdf6992130a49a2252615013980b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978786"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Eastern Standard Time\""));

OutlookTask outlookTask = new OutlookTask();
DateTimeTimeZone dueDateTime = new DateTimeTimeZone();
dueDateTime.dateTime = "2016-05-06T16:00:00";
dueDateTime.timeZone = "Eastern Standard Time";
outlookTask.dueDateTime = dueDateTime;

graphClient.me().outlook().tasks("AAMkADA1MTHgwAAA=")
    .buildRequest( requestOptions )
    .patch(outlookTask);

```