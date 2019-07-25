---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 98f4eb871416d7b03fef78725523938c0d2a89a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892529"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessActivityUserCounts('D7')
    .Request()
    .GetAsync();

```