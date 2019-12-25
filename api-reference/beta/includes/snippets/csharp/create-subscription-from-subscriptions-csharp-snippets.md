---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1d9bf7ffc0cf5992448b1442184277aff08b1af
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870822"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = new Subscription
{
    ChangeType = "updated",
    NotificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    Resource = "me/mailFolders('Inbox')/messages",
    ExpirationDateTime = DateTimeOffset.Parse("2016-11-20T18:23:45.9356913Z"),
    ClientState = "secretClientValue"
};

await graphClient.Subscriptions
    .Request()
    .AddAsync(subscription);

```