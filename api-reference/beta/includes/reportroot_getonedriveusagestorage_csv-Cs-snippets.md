---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5fddd1ab4b3c2df1974335e3a9c1e7bb30b8f6d9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440896"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageStorage = await graphClient.Reports.GetOneDriveUsageStorage('D7')
    .Request()
    .GetAsync();

```