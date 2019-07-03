---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ec497cedfc8d21e493c1fe275f1a1d5ceaa9eaf4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493688"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Groups["{id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```