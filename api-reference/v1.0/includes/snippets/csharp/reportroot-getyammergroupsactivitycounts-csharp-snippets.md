---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ff88f6c3d24955620c09bceb1fb7ac5179ef9c77
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881237"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerGroupsActivityCounts('D7')
    .Request()
    .GetAsync();

```