---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 17354694f582e1439f3078a7b9ec85823350b9d6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718330"
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