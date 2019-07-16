---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cd9a9735cafda014293736223e2b87c0c0fa14b3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735151"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Devices["{id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```