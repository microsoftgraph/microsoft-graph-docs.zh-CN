---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0ac9e4b078a9cf2720bad1b941d3cb559b6e2efe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520065"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Submissions["850f51b7"]
    .Submit()
    .Request()
    .PostAsync();

```