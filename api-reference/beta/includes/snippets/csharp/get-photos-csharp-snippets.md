---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ff2849f23da9b870be81a80f9db9c1428283caed
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var photos = await graphClient.Groups["{id}"].Photos
    .Request()
    .GetAsync();

```