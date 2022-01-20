---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77df7382ca781f342de07e6b6a05ac4fb79d8872
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088191"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userIds = new List<String>()
{
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
};

await graphClient.IdentityProtection.RiskyUsers
    .ConfirmCompromised(userIds)
    .Request()
    .PostAsync();

```