---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e15b2f988df06fe14f1ae1cf9e2b955744fe6da9
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = new Subscription
{
    ChangeType = "created",
    NotificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    Resource = "me/mailFolders('Inbox')/messages",
    ExpirationDateTime = DateTimeOffset.Parse("2016-11-20T18:23:45.9356913Z"),
    ClientState = "secretClientValue",
    LatestSupportedTlsVersion = "v1_2"
};

await graphClient.Subscriptions
    .Request()
    .AddAsync(subscription);

```