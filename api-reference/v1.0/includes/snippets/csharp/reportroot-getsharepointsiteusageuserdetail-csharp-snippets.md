---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b2130287015c57569702c7caf77d74fa7613e3d4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893487"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageDetail('D7')
    .Request()
    .GetAsync();

```