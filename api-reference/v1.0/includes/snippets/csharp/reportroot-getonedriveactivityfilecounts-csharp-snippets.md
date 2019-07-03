---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4f22afbffc3041557485d6527afe84d04c1996e3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOneDriveActivityFileCounts('D7')
    .Request()
    .GetAsync();

```