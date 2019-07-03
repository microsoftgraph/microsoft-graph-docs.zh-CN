---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9453d626b8d5e612ceb0acbd032ffdec5293dace
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509263"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive.Search('{search-query}')
    .Request()
    .GetAsync();

```