---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e58d8200c88c2ee5c5fe6a0f95293c6b1e51442
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccount = new WebAccount
{
    Description = "description-value",
    UserId = "userId-value",
    Service = new ServiceInformation
    {
        Name = "name-value",
        WebUrl = "webUrl-value"
    },
    StatusMessage = "statusMessage-value",
    WebUrl = "webUrl-value"
};

await graphClient.Me.Profile.WebAccounts["{id}"]
    .Request()
    .UpdateAsync(webAccount);

```