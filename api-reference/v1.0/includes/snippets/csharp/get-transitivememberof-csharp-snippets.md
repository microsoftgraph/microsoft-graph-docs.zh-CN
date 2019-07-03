---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 383a6f633a95290ce91ad57573c489c2a3a2b512
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509776"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Me.TransitiveMemberOf
    .Request()
    .GetAsync();

```