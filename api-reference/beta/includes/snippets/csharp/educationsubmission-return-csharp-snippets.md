---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3783e4d3f5585c52b5b75b9ba9bc50460476de03
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478308"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Submissions["850f51b7"]
    .Return()
    .Request()
    .PostAsync();

```