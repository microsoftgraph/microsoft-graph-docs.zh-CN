---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7c443f7690e5d574c914c26c9bc73369c59f5efd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735779"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOneDriveUsageAccountCounts('D7')
    .Request()
    .GetAsync();

```