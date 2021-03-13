---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 677d2dbad40515c22c8af890d55ed312ad53c985
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786599"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.Contacts["{orgContact-id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```