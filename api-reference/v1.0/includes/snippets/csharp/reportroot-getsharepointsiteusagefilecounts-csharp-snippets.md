---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 285b7e45cd16680268208d5b5c8c5bad04c87034
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageFileCounts('D7')
    .Request()
    .GetAsync();

```