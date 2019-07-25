---
description: 自动生成的文件。 不修改
ms.openlocfilehash: af3f5e5ce9757f0ddd9a4d263fed83f40816029a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893403"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsagePages('D7')
    .Request()
    .GetAsync();

```