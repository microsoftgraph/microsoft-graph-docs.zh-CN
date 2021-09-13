---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f3074725c9b673720fa1c8f6187e223bf4cf3610f6b2d67b84acc1bcad1335e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162943"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailboxSettings mailboxSettings = new MailboxSettings();
mailboxSettings.additionalDataManager().put("@odata.context", new JsonPrimitive("https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings"));
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