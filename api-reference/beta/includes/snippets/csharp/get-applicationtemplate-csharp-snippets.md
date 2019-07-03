---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 886da2bf000935b475cbfba040164a3fe3d28ef3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479864"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationTemplate = await graphClient.ApplicationTemplates["{id}"]
    .Request()
    .GetAsync();

```