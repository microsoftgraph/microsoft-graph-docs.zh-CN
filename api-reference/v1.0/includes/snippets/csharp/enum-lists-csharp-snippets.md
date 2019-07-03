---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 068f5dbf853313db72b05ec616cc79333ce671dc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var lists = await graphClient.Sites["{site-id}"].Lists
    .Request()
    .GetAsync();

```