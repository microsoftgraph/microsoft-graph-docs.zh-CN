---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 152f7a97062d537b3f0675b2154e67f5878f9787
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var usageRights = await graphClient.Users["{user-id}"].UsageRights
    .Request()
    .Filter("state in ('active', 'suspended') and serviceIdentifier in ('ABCD')")
    .GetAsync();

```