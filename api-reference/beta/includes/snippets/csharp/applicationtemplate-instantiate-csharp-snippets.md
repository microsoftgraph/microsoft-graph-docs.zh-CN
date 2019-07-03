---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 12a6fb4c469542d31e1e33ec008bde667defdd6c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479982"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "My custom name";

await graphClient.ApplicationTemplates["{id}"]
    .Instantiate(displayName)
    .Request()
    .PostAsync();

```