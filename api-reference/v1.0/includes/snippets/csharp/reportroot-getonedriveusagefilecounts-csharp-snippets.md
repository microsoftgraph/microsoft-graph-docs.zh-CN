---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f515a4f70e963e45952a742bfff47593bea2cd91
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893599"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveUsageFileCounts('D7')
    .Request()
    .GetAsync();

```