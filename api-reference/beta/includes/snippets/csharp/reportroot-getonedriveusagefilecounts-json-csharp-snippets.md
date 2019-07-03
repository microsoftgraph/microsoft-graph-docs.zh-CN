---
description: 自动生成的文件。 不修改
ms.openlocfilehash: efcc5891d38122349b5e233428bb6a614011b260
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519732"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageFileCounts = await graphClient.Reports.GetOneDriveUsageFileCounts('D7')
    .Request()
    .GetAsync();

```