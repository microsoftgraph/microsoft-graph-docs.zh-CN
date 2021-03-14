---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0832016a8074098354c4ec072b16e1e79c1ada00
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.Groups["{group-id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```