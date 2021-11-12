---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 284f9c16f36acbcef041c6691d5f6efa46391028ec6527e96a9683ccd9903262
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162236"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DateTimeTimeZone newReminderTime = new DateTimeTimeZone();
newReminderTime.dateTime = "2016-10-19T10:37:00Z";
newReminderTime.timeZone = "timeZone-value";

graphClient.me().events("{id}")
    .snoozeReminder(EventSnoozeReminderParameterSet
        .newBuilder()
        .withNewReminderTime(newReminderTime)
        .build())
    .buildRequest()
    .post();

```