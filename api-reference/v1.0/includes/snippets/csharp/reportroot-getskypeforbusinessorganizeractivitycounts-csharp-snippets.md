---
description: 自动生成的文件。 不修改
ms.openlocfilehash: db331133db79b2b0afab6149b927f7e854e90d36
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892349"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityCounts('D7')
    .Request()
    .GetAsync();

```