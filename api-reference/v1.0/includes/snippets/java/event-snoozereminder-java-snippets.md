---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd7a2bca064f6b1ff35b4f1bcfdb16e152e4444c822e48fabba0451935c84e4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274251"
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