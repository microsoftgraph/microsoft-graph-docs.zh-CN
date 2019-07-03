---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0277ad0b4d98e12104de08784b5daccf42c74c86
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520516"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityUserCounts = await graphClient.Reports.GetOneDriveActivityUserCounts('D7')
    .Request()
    .GetAsync();

```