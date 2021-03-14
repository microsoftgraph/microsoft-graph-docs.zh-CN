---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0b2718ffc957b2d884016780b90e36b0f04b054
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = false;

await graphClient.Groups["{group-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```