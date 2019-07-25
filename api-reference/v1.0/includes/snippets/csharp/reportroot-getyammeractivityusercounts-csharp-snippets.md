---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 24f4b75a3ce7d4ffdda3f1415af6bf5df65b3da0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```