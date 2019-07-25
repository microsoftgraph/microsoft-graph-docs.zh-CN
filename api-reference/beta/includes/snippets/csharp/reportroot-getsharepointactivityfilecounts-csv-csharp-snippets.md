---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4bc643d9679acd60a8d47db55c766797a288d5d7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872876"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityFileCounts = await graphClient.Reports
    .GetSharePointActivityFileCounts('D7')
    .Request()
    .GetAsync();

```