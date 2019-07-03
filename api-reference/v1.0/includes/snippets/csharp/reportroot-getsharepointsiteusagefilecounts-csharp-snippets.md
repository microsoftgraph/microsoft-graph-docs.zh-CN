---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83a0b5d4759c9a6d153acc8f3128401c6d60a912
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492963"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointSiteUsageFileCounts('D7')
    .Request()
    .GetAsync();

```