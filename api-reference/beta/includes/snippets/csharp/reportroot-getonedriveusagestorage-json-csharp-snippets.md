---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5fddd1ab4b3c2df1974335e3a9c1e7bb30b8f6d9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageStorage = await graphClient.Reports.GetOneDriveUsageStorage('D7')
    .Request()
    .GetAsync();

```