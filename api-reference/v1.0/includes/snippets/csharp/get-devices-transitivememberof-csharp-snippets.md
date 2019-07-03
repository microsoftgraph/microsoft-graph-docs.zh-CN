---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cd9a9735cafda014293736223e2b87c0c0fa14b3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509186"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Devices["{id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```