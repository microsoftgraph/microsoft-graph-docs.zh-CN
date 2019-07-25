---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 45008f17bddcba3ac45fc17479307c2ff90eec76
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessOrganizerActivityUserCounts = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```