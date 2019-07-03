---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ac7a5220305ade46784fe47cf9ca27499b8a93b1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupSettings["{id}"]
    .Request()
    .DeleteAsync();

```