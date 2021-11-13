---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b1e31ccc8523bc93e4478d1f136f2ee3028e0b6
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890545"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var submissions = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions
    .Request()
    .Expand("outcomes")
    .GetAsync();

```