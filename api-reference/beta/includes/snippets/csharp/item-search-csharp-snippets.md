---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0c7bea8e42da208414aa485f10951b3dfa5030da
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500267"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive.Root.Search('{search-query}')
    .Request()
    .GetAsync();

```