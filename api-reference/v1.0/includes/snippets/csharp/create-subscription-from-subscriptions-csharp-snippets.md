---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 165fed6073a7d4b72867de86439db23b67a6e1cdb2bb9c793895ac6e694c9d56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161993"
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