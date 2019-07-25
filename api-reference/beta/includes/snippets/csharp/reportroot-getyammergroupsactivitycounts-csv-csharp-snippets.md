---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2390e8a25d318068aaa8f814f0842b92910fa984
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871340"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerGroupsActivityCounts = await graphClient.Reports
    .GetYammerGroupsActivityCounts('D7')
    .Request()
    .GetAsync();

```