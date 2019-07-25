---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b67c86f6bc83bdf6992130a49a2252615013980b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877659"
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