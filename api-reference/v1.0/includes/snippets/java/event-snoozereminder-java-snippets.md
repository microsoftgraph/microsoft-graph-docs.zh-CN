---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8721e3bc2c151ee301a9436d9d95e1238b5b4d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976067"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DateTimeTimeZone newReminderTime = new DateTimeTimeZone();
newReminderTime.dateTime = "dateTime-value";
newReminderTime.timeZone = "timeZone-value";

graphClient.me().events("{id}")
    .snoozeReminder(EventSnoozeReminderParameterSet
        .newBuilder()
        .withNewReminderTime(newReminderTime)
        .build())
    .buildRequest()
    .post();

```