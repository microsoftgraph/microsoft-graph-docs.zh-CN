---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8b15df0c2215d0c64f496def60ab10b86111def3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityCounts('D7')
    .Request()
    .GetAsync();

```