---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eab6ebe01d30d7fe903981bf9e1b3a3f582b0e44
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982715"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailboxSettings mailboxSettings = new MailboxSettings();
mailboxSettings.additionalDataManager().put("@odata.context", new JsonPrimitive("https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings"));
AutomaticRepliesSetting automaticRepliesSetting = new AutomaticRepliesSetting();
automaticRepliesSetting.status = AutomaticRepliesStatus.SCHEDULED;
DateTimeTimeZone scheduledStartDateTime = new DateTimeTimeZone();
scheduledStartDateTime.dateTime = "2016-03-20T18:00:00";
scheduledStartDateTime.timeZone = "UTC";
automaticRepliesSetting.scheduledStartDateTime = scheduledStartDateTime;
DateTimeTimeZone scheduledEndDateTime = new DateTimeTimeZone();
scheduledEndDateTime.dateTime = "2016-03-28T18:00:00";
scheduledEndDateTime.timeZone = "UTC";
automaticRepliesSetting.scheduledEndDateTime = scheduledEndDateTime;
mailboxSettings.automaticRepliesSetting = automaticRepliesSetting;

graphClient.customRequest("/me/mailboxSettings", MailboxSettings.class)
    .buildRequest()
    .patch(mailboxSettings);

```