---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bfea13fdd0a8688345d560c93604a612d89208d5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881027"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerActivityUserDetail('D7')
    .Request()
    .GetAsync();

```