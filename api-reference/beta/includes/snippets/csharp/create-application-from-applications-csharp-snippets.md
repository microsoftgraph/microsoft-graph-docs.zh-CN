---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 34b448da31da5368d723339d7e9b6129f5dbbd00
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    AllowPublicClient = true,
    DisplayName = "Display name"
};

await graphClient.Applications
    .Request()
    .AddAsync(application);

```