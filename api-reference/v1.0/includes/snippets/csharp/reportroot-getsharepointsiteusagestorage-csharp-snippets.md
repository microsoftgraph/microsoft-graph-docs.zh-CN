---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4ea23e1a3c90e8e3a373d59ad6656926ad9444a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893347"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageStorage('D7')
    .Request()
    .GetAsync();

```