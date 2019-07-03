---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e052f9abc42dcdd357eaeef31f818b72cdca9957
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"]
    .Publish()
    .Request()
    .PostAsync();

```