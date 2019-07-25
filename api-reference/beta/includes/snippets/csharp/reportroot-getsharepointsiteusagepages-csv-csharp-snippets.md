---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 57662ac838c722dae0428fd99d673a4a7eda3f86
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsagePages = await graphClient.Reports
    .GetSharePointSiteUsagePages('D7')
    .Request()
    .GetAsync();

```