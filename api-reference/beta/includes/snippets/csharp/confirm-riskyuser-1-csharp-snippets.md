---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17354694f582e1439f3078a7b9ec85823350b9d6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950487"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userIds = new List<String>()
{
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
};

await graphClient.RiskyUsers
    .ConfirmCompromised(userIds)
    .Request()
    .PostAsync();

```