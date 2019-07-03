---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d23dc968d33e2279a2ec6f270756ca6a96738296
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySetting = await graphClient.Settings["{id}"]
    .Request()
    .GetAsync();

```