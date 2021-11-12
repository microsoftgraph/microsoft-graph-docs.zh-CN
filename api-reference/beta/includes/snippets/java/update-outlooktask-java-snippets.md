---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca9beb8f29800d13587b9afece47a2662e0ac8e05232a9b553f9bd3687240bbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163662"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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